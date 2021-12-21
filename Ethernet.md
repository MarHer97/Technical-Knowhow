<a name="top"></a>
# Ethernet

<br/>

Inhalt des Markdowns Ethernet

**[01 Definition](#01)** <br/>
**[02 Funktionsweise](#02)** <br/>
**[03 Standard](#03)** <br/>
> [OSI Model](#03.1) <br/>

**[04 Bitübertragungsschicht (Physical Layer)](#04)** <br/>
> [Ethernet Verkabelung](#04.1) <br/>
> [Ethernet Geräte](#04.1) <br/>


**[04 Sicherungsschicht (Data Link Layer)](#05)** <br/>
> [Logical Link Control (LLC)](#05.1) <br/>
> [Meadia Access Controll (MAC)](#05.2) <br/>


<br/>

<br/>

<br/>

#### Begriffe

| Begriff                                             | Erklärung                                                                                                                                   |
| :----------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------- |
| LAN (Local Area Network)                                    | Rechnernetz, das mehrere Systeme lokal miteinander verbindet                                                                                |
| Switching                                                   | Switching regelt den Weg eines Datenpakets im Netzwerk; Eingang und Ausgang von Paketen werden je nach Sender und Empfänger festgelegt      |
| Ethernet Flow Control                                       | Datenübertragung im Ethernet wird temporär gestoppt; Ziel ist weniger Datenverlust und mehr Effizienz                                       |
| CSMA/CD (Carrier Sense Multiple Access/Collision Detection) | Medienzugriffsverfahren, das festlegt, welche Systeme in einem Netzwerk auf ein Übertragungsmedium zugreifen dürfen; verhindert Kollisionen |
| Ethernet-Frame/Datenframe                                   | Protokolleinheit, die wichtige Informationen für die Datenübermittlung enthalt, u. a. die MAC-Adresse                                       |
| MAC-Adresse/Geräteadresse                                   | Einzigartige zugewiesene Adresse eines Geräts im Rechnernetz                                                                                |
| PoE (Power over Ethernet)                                   | Das Ethernet-Kabel kann das Zielgerät mit Strom versorgen                                                                                   |
| Koaxialkabel                                                | Zweipoliges Kabel, bis zu 10 Mbit/s (veraltete Technik)                                                                                     |
| Twisted-Pair-Kabel                                          | Kabel mit verdrillten Aderpaaren, ermöglicht PoE, bis zu 10 Gbit/s                                                                          |
| Glasfaserkabel                                              | Lichtwellenleiter, hohe Reichweite, enorme Übertragungsraten möglich (theoretisch schon bis ca. 70 Terabit/s)                               |
| Halbduplexmodus                                             | Kommunikation ist nur abwechselnd in eine Richtung möglich (veraltete Technik)                                                              |
| Vollduplexmodus                                             | Kommunikation ist gleichzeitig in beide Richtungen möglich                                                                                  |
<br/>

<br/>

<br/>

<a name="01"></a>
## 01 Definition
**Ethernet ist ein Kommunikationsstandard welcher in den frühen 1980er Jahren entwickelt wurde, um Computer und andere Geräte in einer lokalen Umgebung wie in einem Haus oder einem Gebäude zu vernetzen. Diese lokale Umgebung wird als LAN oder Local Area Network definiert. Ethernet verbindet mehrere Geräte, damit diese Informationen erstellen, speichern und mit anderen Geräten innerhalb der lokalen Umgebung teilen können.**

Ethernet ist ein kabelgebundenes System, welches mit der Verwendung von Koaxialkabeln (Coaxial Cable) begann und sich heute erfolgreich mit Twisted Pair Kupferkabeln (Twisted Pair Cable) und Glasfaserkabeln (Fiber Optic Cable) entwickelt hat.


**Das Ethernet bezeichnet eine Technik für kabelgebundene Datennetze, die Software und/oder Hardware miteinander verbindet. Das geschieht meist über LAN-Kabel, deshalb wird Ethernet auch häufig als LAN-Technik angeführt. Ethernet erlaubt so den Datenaustausch zwischen Endgeräten. Das können Computer, Drucker, Server, Verteiler usw. sein.** Zusammengeschlossen in einem lokalen Netzwerk stellen diese Geräte somit Verbindungen über das Ethernet-Protokoll her und können Datenpakete untereinander austauschen. Das aktuelle und am weitesten verbreitete Protokoll dafür ist IEEE 802.3.


Während die erste Version der Technik nur 3 Megabit pro Sekunde schnell war, ermöglichen heute Ethernet-Protokolle Geschwindigkeiten bzw. von Übertragungsraten von 1, 10, 100 Megabit/s (Fast Ethernet), 1000 Megabit/s (Gigabit-Ethernet). Frühe Ethernets waren auf ein Gebäude beschränkt, heute kann Ethernet über Glasfaser bis zu 10 Kilometer abdecken. Ethernet-Standard-Varianten über Glasfaser haben eine Reichweite von bis zu 70 km, proprietäre auch mehr.

&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<br/>

<a name="02"></a>
## 02 Funktionsweise
**Jedes Gerät in einem Ethernet-Netzwerk bekommt eine eigene Adresse zugewiesen, die man [MAC-Adresse](https://www.ionos.de/digitalguide/server/knowhow/mac-adresse/) (48-Bit) nennt. Die Mitglieder in diesem gemeinsamen Netzwerk können Nachrichten durch Hochfrequenz übertragen. **Ethernet verwendet dafür das Basisbandverfahren und das Multiplexverfahren. Für die Kommunikation untereinander wird der reibungslose Algorithmus [CSMA/CD](https://www.ionos.de/digitalguide/server/knowhow/csmacd-carrier-sense-multiple-access-collision-detection/) (Carrier Sense Multiple Access/Collision Detection) verwendet. Die Netzwerk-Topologie von Ethernet ist logisch, also kann der Aufbau z. B. als Bus oder Stern realisiert werden.


Die Kommunikation mit diesem Algorithmus [CSMA/CD](https://www.ionos.de/digitalguide/server/knowhow/csmacd-carrier-sense-multiple-access-collision-detection/) (Carrier Sense Multiple Access/Collision Detection) ist ähnlich einer Gesprächsrunde, bei der jeder Teilnehmer den anderen ausreden lässt. Kollidieren zwei Nachrichten, versuchen die Teilnehmer in zufälligen Abständen eine erneute Übertragung. Weil für eine erfolgreiche Kommunikation sowohl gesendet als auch empfangen werden muss, darf es nicht zum Datenstau kommen, etwa wenn eine gesendete Nachricht zu stark für eine eher schwache Empfangsleistung ist. Ansonsten können Daten verloren gehen. Signalgeschwindigkeit und Übertragungsrate regeln das reibungslose Kommunizieren, indem Regeln für die Datenframes festgelegt werden.

Damit eine Kollision von Daten verhindert wird, muss ein entsprechendes Störsignal vor dem Datenpaket beim Empfänger ankommen. Weil heutzutage die meisten Netzwerke im Vollduplexmodus funktionieren, ist dieses Problem jedoch nur selten anzutreffen. Es war jedoch wesentlich für die frühe Entwicklung der Ethernet-Technik.


&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<br/>

<a name="03"></a>
## 03 Standard
**Im Jahr 1983 wurde Ethernet vom Instutute of Electrical and Electronic Engineers (IEEE) in den Standard IEEE 802.3 standardisiert.**

Ethernet entspricht weitestgehend der IEEE-Norm 802.3. Es wurde ab den 1990ern zur meistverwendeten LAN-Technik und hat andere LAN-Standards wie Token Ring verdrängt oder, wie im Falle von ARCNET in Industrie- und Fertigungsnetzen oder FDDI in hoch verfügbaren Netzwerken, zu Nischenprodukten für Spezialgebiete gemacht.

**Die Norm IEEE 802.3 definiert die physikalische Schicht (Physical Layer) und den MAC (Media Access Control) der Sicherungsschicht (Data Link Layer) von drahtgebundenem Ethernet.** 

<img src="https://user-images.githubusercontent.com/83710723/146945009-3b0c0a1a-4af9-4a96-ada0-729f4b57de0d.png" alt="drawing" width="500"/>

<br/>

**Übersicht der wichtigsten [IEEE 802.3 Normenteile](https://de.wikipedia.org/wiki/IEEE_802)**


| Ethernet-Standard | Bezeichnung                                                                         | Datenrate  | Kabeltechnik                       | Erscheinungsjahr |
| :----------------- | :----------------------------------------------------------------------------------- | :---------- | :---------------------------------- | :---------------- |
| 802.3             | 10Base5                                                                             | 10 Mbit/s  | Koaxialkabel                       | 1983             |
| 802.3a            | [10Base2](https://de.wikipedia.org/wiki/10BASE2)                                                                             | 10 Mbit/s  | Koaxialkabel                       | 1988             |
| 802.3i            | [10Base-T](https://de.wikipedia.org/wiki/Ethernet#10-Mbit/s-Ethernet_mit_Twisted-Pair-Kabel)                                                                            | 10 Mbit/s  | Twisted-Pair-Kabel                 | 1990             |
| 802.3j            | 10Base-FL                                                                           | 10 Mbit/s  | Glasfaserkabel                     | 1992             |
| 802.3u            | 100Base-TX, 100Base-FX, 100Base-SX, [Fast Ethernet](https://de.wikipedia.org/wiki/Ethernet#100-Mbit/s-Ethernet)                                                  | 100 Mbit/s | Twisted-Pair-Kabel, Glasfaserkabel | 1995             |
| 802.3z            | 1000Base-SX, 1000Base-LX, [Gigabit Ethernet über Glasfaser](https://de.wikipedia.org/wiki/Ethernet#Gigabit-Ethernet)                                                           | 1 Gbit/s   | Glasfaserkabel                     | 1998             |
| 802.3ab           | 1000Base-T                                                                          | 1 Gbit/s   | Twisted-Pair-Kabel                 | 1999             |
| 802.3ae           | 10GBase-SR, 10GBase-SW, 10GBase-LR, 10GBase-LW, 10GBase-ER, 10GBase-EW, 10GBase-LX4, [10-Gigabit-Ethernet](https://de.wikipedia.org/wiki/Ethernet#10-Gbit/s-Ethernet) | 10 Gbit/s  | Glasfaserkabel                     | 2002             |
| 802.an            | [10GBase-T](https://de.wikipedia.org/wiki/IEEE_802.3an)                                                                           | 10 Gbit/s  | Twisted-Pair-Kabel                 | 2006             |

<br/>

**Weitere neuset Erweiterungen der [IEEE 802.3 Normenteile](https://de.wikipedia.org/wiki/IEEE_802)**
- 802.3af – [Power over Ethernet](https://de.wikipedia.org/wiki/Power_over_Ethernet)
- 802.3at – [Power over Ethernet](https://de.wikipedia.org/wiki/Power_over_Ethernet)
- 802.3az – [Energy Efficient Ethernet](https://de.wikipedia.org/wiki/Energy_Efficient_Ethernet)
- 802.3ba – 100 Gigabit Ethernet



&uarr; [zurück zum Seitenanfang](#top)


<br/>

<br/>

<a name="03.1"></a>
### OSI Model
Das ISO/OSI-Referenzmodell (Open Systems Interconnection model) ist ein Referenzmodell für Netzwerkprotokolle als Schichtenarchitektur. Es wird seit 1983 von der International Telecommunication Union (ITU) und seit 1984 auch von der International Organization for Standardization (ISO) als Standard veröffentlicht. Seine Entwicklung begann im Jahr 1977.

Zweck des OSI-Modells ist es, Kommunikation über unterschiedlichste technische Systeme hinweg zu beschreiben und die Weiterentwicklung zu begünstigen. Dazu definiert dieses Modell sieben aufeinanderfolgende Schichten (engl. layers) mit jeweils eng begrenzten Aufgaben. In der gleichen Schicht mit klaren Schnittstellen definierte Netzwerkprotokolle sind einfach untereinander austauschbar, selbst wenn sie wie das Internet Protocol eine zentrale Funktion haben.

**Im OSI-Modell ist mit Ethernet sowohl die [physische Schicht](url) (OSI Layer 1 bzw. Bitübertragungsschicht) als auch die [Data-Link-Schicht](url) (OSI Layer 2 bzw. Sicherungsschicht) festgelegt.**

<img src="https://user-images.githubusercontent.com/83710723/146954345-197f3268-7283-4180-844b-ae239adfa0e2.png" alt="drawing" width="500"/>


&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<br/>

<a name="04"></a>
## 04 Bitübertragungsschicht (Physical Layer)
Die Bitübertragungsschicht (engl. Physical Layer) ist die unterste Schicht. Diese Schicht stellt mechanische, elektrische und weitere funktionale Hilfsmittel zur Verfügung, um physische Verbindungen zu aktivieren bzw. zu deaktivieren, sie aufrechtzuerhalten und Bits darüber zu übertragen.

<br/>

<br/>

<a name="04.1"></a>
### Ethernet Verkabelung
**Ethernet ist ein kabelgebundenes System, welches mit der Verwendung von Koaxialkabeln (Coaxial Cable) begann und sich heute erfolgreich mit Twisted Pair Kupferkabeln (Twisted Pair Cable) und Glasfaserkabeln (Fiber Optic Cable) entwickelt hat.** Koaxialkabel sind heute nicht mehr weit verbreitet, außer in älteren Installationen. Die am häufigsten verwendeten Kabel sind Twisted Pair Kupferkabel.

<br/>

#### Twisted Pair Kupferkabel

<br/>


**Kategorien der Twisted Pair Kupferkabel** <br/>

<img src="https://user-images.githubusercontent.com/83710723/146945949-879b2f13-42cf-4a0d-9b2d-4a2ddd501e4d.png" alt="drawing" width="500"/>

Kabel der Kategorie 5 und 5e werden beide noch in vielen bestehenden Anwendungen verwendet, verarbeiten jedoch die niedrigeren Gewschwindigkeiten zwischen 10 Mbit/s und 100 Mbits/s, sind aber anfälliger für Rauschen.

<br/>

**Ethernet PIN Anschlüsse** <br/>

Das Twisted Pair Kupferkabel verwendet RJ 45 8 PIN Anschlüsse an beiden Enden des Kabels, die zum Senden und Empfangen von Daten im Halb- oder Vollduplexmodus gepinnt sind.

Halbduplex überträgt Daten in eine Richtung gleichzeitig, während Vollduplex die gleichzeitige Übertragung von Daten in beide Richtungen ermöglicht. Vollduplex kann in Ethernet erreicht werden, indem zwei Adrenpaare verwendet werden, damit Daten gleichzeitig in beide Richtungen übertragen werden können.


&uarr; [zurück zum Seitenanfang](#top)

<br/>

#### Glasfaserkabeln (Fiber Optic Cable)
Glasfaserkabel verwenden optische Glasfasern aus Glas oder Kunststoff als Leitung für Lichtimpulse zur Übertragung von Daten. Dies hat Ethernet ermöglicht, größere Entfernungen mit höheren Geschwindigkeiten zu überwinden.

<img src="https://user-images.githubusercontent.com/83710723/146947895-8d147429-ea17-4511-b52d-816ce80b7118.png" alt="drawing" width="500"/>


<br/>


**Kategorien der Glasfaserkabeln** <br/>
Glasfaserkabel verwenden verschiedene Arten von Steckverbindern, die je nach Anwendungsanforderungen variieren:
- SFP Connector (Small Form Pluggable)
- SC Connector (Subscriber Connector oder Standard Connector) 

<img src="https://user-images.githubusercontent.com/83710723/146948164-8cf45c7a-4911-41b3-b3f0-ba9df1f6fc97.png" alt="drawing" width="500"/>


Um Glasfaser in einem Ethernet-Netzwerk zu verwenden, welches Twisted Pair Kupferkabel verwendet, müssen Sie einen Ethernet zu Glasfaser Konverter verwenden. Damit wird es dem Netzwerk ermöglicht die höheren Geschwindigkeiten von Glasfaser zu nutzen und die Entfernung zu verlängern, die das Ethernet Netzwerk erreichen kann.

<img src="https://user-images.githubusercontent.com/83710723/146948809-1cf5477e-214f-4236-9d8f-aea6265c5f6f.png" alt="drawing" width="500"/>


&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<a name="04.2"></a>
### Ethernet Geräte
**Ethernet Geräte bestehen aus Computern, Druckern oder andere Geräte, die entweder über eine interne NIC (Network Interface Card) oder eine externe NIC (Network Interface Card) die auf USB oder PCI basiert. Switches und Router, die als Direktor des Netzwerkes fungieren und mehrere Computer oder sogar Netzwerke miteinander verbinden, um die Kommunikation zwischen all den verschiedenen Geräten zu ermöglichen.**

<img src="https://user-images.githubusercontent.com/83710723/146950135-af6272d0-f21d-4419-87fc-8fcf7524e69d.png" alt="drawing" width="500"/>

Gateways und Bridges werden verwendet, um mehrere Ethernet Netzwerk miteinander zu verbinden und die Kommunikation über das lokale Netzwerk hinweg zu ermöglichen. Gateways verbinden zwei unterschiedliche Netzwerke miteinander, während eine Bridge zwei ähnliche Netzwerke miteinander verbindet, sodass Sie nur ein Netzwerk sehen.

&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<br/>

<a name="05"></a>
## 05 Sicherungsschicht (Data Link Layer)
Aufgabe der Sicherungsschicht (engl. Data Link Layer; auch Abschnittssicherungsschicht, Datensicherungsschicht, Verbindungssicherungsschicht, Verbindungsebene, Prozedurebene) ist es, eine zuverlässige, das heißt weitgehend fehlerfreie Übertragung zu gewährleisten und den Zugriff auf das Übertragungsmedium zu regeln. 

**Ethernet überträgt Datenpakete in dieser Sicherungsschicht mithilfe eines Algorithumus mit der Bezeichnung CSMA/CD (Carrier Sense Multiple Access with Collision Detection). CSMA/CD wird als Standard für Ethernet verwendet, um Datenkollisionen zu reduzieren und die erfolgreiche Datenübertragung zu erhöhen.** Der Algorithumus überprüft zunächst ob Datenverkehr im Netzwerk vorhanden ist.

Die Sicherungsschicht kann in zwei Abschnitte unterteilt werden:

<img src="https://user-images.githubusercontent.com/83710723/146955067-5f40b002-283f-445e-baaa-bf296575baa8.png" width="500"/>


<br/>

<br/>

<a name="05.1"></a>
### Logical Link Control (LLC)
Die Logical Link Control (LLC) erstellt Pfade für Daten auf dem Ethernet, um zwischen Geräten zu übertragen.

&uarr; [zurück zum Seitenanfang](#top)


<br/>

<br/>

<a name="05.2"></a>
### Meadia Access Controll (MAC)
Die Meadia Access Controll (MAC) verwendet Hardwareadressdaten, die Netzwerkschnittstellenkarten (NIC) zugewiesen sind, um einen bestimmten Comuputer oder ein bestimmtes Gerät zu identifizieren und die Quelle und das Ziel von Datenübertragungen anzuzeigen.

&uarr; [zurück zum Seitenanfang](#top)

<br/>
