<a name="top"></a>
# Ethernet

<br/>

Inhalt des Markdowns Ethernet

**[01 Definition](#01)** <br/>
**[02 Standard](#02)** <br/>
**[03 Voraussetzungen](#03)** <br/>
**[04 Standards](#04)** <br/>



<br/>

<br/>

<br/>

<a name="01"></a>
## 01 Definition
**Ethernet ist ein Kommunikationsstandard welcher in den frühen 1980er Jahren entwickelt wurde, um Computer und andere Geräte in einer lokalen Umgebung wie in einem Haus oder einem Gebäude zu vernetzen. Diese lokale Umgebung wird als LAN oder Local Area Network definiert. Ethernet verbindet mehrere Geräte, damit diese Informationen erstellen, speichern und mit anderen Geräten innerhalb der lokalen Umgebung teilen können.**

Ethernet ist ein kabelgebundenes System, welches mit der Verwendung von Koaxialkabeln (Coaxial Cable) begann und sich heute erfolgreich mit Twisted Pair Kupferkabeln (Twisted Pair Cable) und Glasfaserkabeln (Fiber Optic Cable) entwickelt hat.


**Ethernet ist eine Technik, die Software (Protokolle usw.) und Hardware (Kabel, Verteiler, Netzwerkkarten usw.) für kabelgebundene Datennetze spezifiziert, welche ursprünglich für lokale Datennetze (LANs) gedacht war und daher auch als LAN-Technik bezeichnet wird. Sie ermöglicht den Datenaustausch in Form von Datenframes zwischen den in einem lokalen Netz (LAN) angeschlossenen Geräten (Computer, Drucker und dergleichen).** Derzeit sind Übertragungsraten von 1, 10, 100 Megabit/s (Fast Ethernet), 1000 Megabit/s (Gigabit-Ethernet), 2,5, 5, 10, 25, 40, 50, 100, 200 und 400 Gigabit/s spezifiziert. In seiner ursprünglichen Form erstreckt sich das LAN dabei nur über ein Gebäude; Ethernet-Standard-Varianten über Glasfaser haben eine Reichweite von bis zu 70 km, proprietäre auch mehr.

Die Ethernet-Protokolle umfassen Festlegungen für Kabeltypen und Stecker sowie für Übertragungsformen (Signale auf der Bitübertragungsschicht, Paketformate). Im OSI-Modell ist mit Ethernet sowohl die physische Schicht (OSI Layer 1) als auch die Data-Link-Schicht (OSI Layer 2) festgelegt. 

 Ethernet kann die Basis für Netzwerkprotokolle, wie z. B. AppleTalk, DECnet, IPX/SPX und TCP/IP, bilden.

Für Anwendungen, in denen hohe Anforderungen an die Zuverlässigkeit der Kommunikation gestellt werden, kommt Echtzeit-Ethernet zum Einsatz.[3]

&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<br/>

<a name="02"></a>
## 02 Standard
**Im Jahr 1983 wurde Ethernet vom Instutute of Electrical and Electronic Engineers (IEEE) in den Standard IEEE 802.3 standardisiert.**

Ethernet entspricht weitestgehend der IEEE-Norm 802.3. Es wurde ab den 1990ern zur meistverwendeten LAN-Technik und hat andere LAN-Standards wie Token Ring verdrängt oder, wie im Falle von ARCNET in Industrie- und Fertigungsnetzen oder FDDI in hoch verfügbaren Netzwerken, zu Nischenprodukten für Spezialgebiete gemacht.

**Die Norm IEEE 802.3 definiert die physikalische Schicht (Physical Layer) und den MAC (Media Access Control) der Sicherungsschicht (Data Link Layer) von drahtgebundenem Ethernet.** 

![image](https://user-images.githubusercontent.com/83710723/146945009-3b0c0a1a-4af9-4a96-ada0-729f4b57de0d.png)

Der Physical Layer besteht aus den folgenden Komponenten:

![image](https://user-images.githubusercontent.com/83710723/146945339-0768fbd6-52a7-424d-94cc-2fbbd0881993.png)

<br/>

<br/>

<a name="02.1"></a>
### OSI Model
Das ISO/OSI-Referenzmodell (Open Systems Interconnection model) ist ein Referenzmodell für Netzwerkprotokolle als Schichtenarchitektur. Es wird seit 1983 von der International Telecommunication Union (ITU) und seit 1984 auch von der International Organization for Standardization (ISO) als Standard veröffentlicht. Seine Entwicklung begann im Jahr 1977.

Zweck des OSI-Modells ist es, Kommunikation über unterschiedlichste technische Systeme hinweg zu beschreiben und die Weiterentwicklung zu begünstigen. Dazu definiert dieses Modell sieben aufeinanderfolgende Schichten (engl. layers) mit jeweils eng begrenzten Aufgaben. In der gleichen Schicht mit klaren Schnittstellen definierte Netzwerkprotokolle sind einfach untereinander austauschbar, selbst wenn sie wie das Internet Protocol eine zentrale Funktion haben.

**Im OSI-Modell ist mit Ethernet sowohl die [physische Schicht](url) (OSI Layer 1 bzw. Bitübertragungsschicht) als auch die [Data-Link-Schicht](url) (OSI Layer 2 bzw. Sicherungsschicht) festgelegt.**

![image](https://user-images.githubusercontent.com/83710723/146954345-197f3268-7283-4180-844b-ae239adfa0e2.png)


&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<br/>

<a name="03"></a>
## 03 Bitübertragungsschicht (Physical Layer)
Die Bitübertragungsschicht (engl. Physical Layer) ist die unterste Schicht. Diese Schicht stellt mechanische, elektrische und weitere funktionale Hilfsmittel zur Verfügung, um physische Verbindungen zu aktivieren bzw. zu deaktivieren, sie aufrechtzuerhalten und Bits darüber zu übertragen.

<br/>

<br/>

<a name="03.1"></a>
### Ethernet Verkabelung
**Ethernet ist ein kabelgebundenes System, welches mit der Verwendung von Koaxialkabeln (Coaxial Cable) begann und sich heute erfolgreich mit Twisted Pair Kupferkabeln (Twisted Pair Cable) und Glasfaserkabeln (Fiber Optic Cable) entwickelt hat.** Koaxialkabel sind heute nicht mehr weit verbreitet, außer in älteren Installationen. Die am häufigsten verwendeten Kabel sind Twisted Pair Kupferkabel.

<br/>

#### Twisted Pair Kupferkabel

<br/>


**Kategorien der Twisted Pair Kupferkabel** <br/>

![image](https://user-images.githubusercontent.com/83710723/146945949-879b2f13-42cf-4a0d-9b2d-4a2ddd501e4d.png)

Kabel der Kategorie 5 und 5e werden beide noch in vielen bestehenden Anwendungen verwendet, verarbeiten jedoch die niedrigeren Gewschwindigkeiten zwischen 10 Mbit/s und 100 Mbits/s, sind aber anfälliger für Rauschen.

<br/>

**Ethernet PIN Anschlüsse** <br/>

Das Twisted Pair Kupferkabel verwendet RJ 45 8 PIN Anschlüsse an beiden Enden des Kabels, die zum Senden und Empfangen von Daten im Halb- oder Vollduplexmodus gepinnt sind.

Halbduplex überträgt Daten in eine Richtung gleichzeitig, während Vollduplex die gleichzeitige Übertragung von Daten in beide Richtungen ermöglicht. Vollduplex kann in Ethernet erreicht werden, indem zwei Adrenpaare verwendet werden, damit Daten gleichzeitig in beide Richtungen übertragen werden können.


&uarr; [zurück zum Seitenanfang](#top)

<br/>

#### Glasfaserkabeln (Fiber Optic Cable)
Glasfaserkabel verwenden optische Glasfasern aus Glas oder Kunststoff als Leitung für Lichtimpulse zur Übertragung von Daten. Dies hat Ethernet ermöglicht, größere Entfernungen mit höheren Geschwindigkeiten zu überwinden.

![image](https://user-images.githubusercontent.com/83710723/146947895-8d147429-ea17-4511-b52d-816ce80b7118.png)

<br/>


**Kategorien der Glasfaserkabeln** <br/>
Glasfaserkabel verwenden verschiedene Arten von Steckverbindern, die je nach Anwendungsanforderungen variieren:
- SFP Connector (Small Form Pluggable)
- SC Connector (Subscriber Connector oder Standard Connector) 

![image](https://user-images.githubusercontent.com/83710723/146948164-8cf45c7a-4911-41b3-b3f0-ba9df1f6fc97.png)

Um Glasfaser in einem Ethernet-Netzwerk zu verwenden, welches Twisted Pair Kupferkabel verwendet, müssen Sie einen Ethernet zu Glasfaser Konverter verwenden. Damit wird es dem Netzwerk ermöglicht die höheren Geschwindigkeiten von Glasfaser zu nutzen und die Entfernung zu verlängern, die das Ethernet Netzwerk erreichen kann.

![image](https://user-images.githubusercontent.com/83710723/146948809-1cf5477e-214f-4236-9d8f-aea6265c5f6f.png)

&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<a name="03.2"></a>
### Ethernet Geräte
**Ethernet Geräte bestehen aus Computern, Druckern oder andere Geräte, die entweder über eine interne NIC (Network Interface Card) oder eine externe NIC (Network Interface Card) die auf USB oder PCI basiert. Switches und Router, die als Direktor des Netzwerkes fungieren und mehrere Computer oder sogar Netzwerke miteinander verbinden, um die Kommunikation zwischen all den verschiedenen Geräten zu ermöglichen.**


![image](https://user-images.githubusercontent.com/83710723/146950135-af6272d0-f21d-4419-87fc-8fcf7524e69d.png)

Gateways und Bridges werden verwendet, um mehrere Ethernet Netzwerk miteinander zu verbinden und die Kommunikation über das lokale Netzwerk hinweg zu ermöglichen. Gateways verbinden zwei unterschiedliche Netzwerke miteinander, während eine Bridge zwei ähnliche Netzwerke miteinander verbindet, sodass Sie nur ein Netzwerk sehen.

&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<br/>

<a name="04"></a>
## 04 Sicherungsschicht (Data Link Layer)
Aufgabe der Sicherungsschicht (engl. Data Link Layer; auch Abschnittssicherungsschicht, Datensicherungsschicht, Verbindungssicherungsschicht, Verbindungsebene, Prozedurebene) ist es, eine zuverlässige, das heißt weitgehend fehlerfreie Übertragung zu gewährleisten und den Zugriff auf das Übertragungsmedium zu regeln. 

**Ethernet überträgt Datenpakete in dieser Sicherungsschicht mithilfe eines Algorithumus mit der Bezeichnung CSMA/CD (Carrier Sense Multiple Access with Collision Detection). CSMA/CD wird als Standard für Ethernet verwendet, um Datenkollisionen zu reduzieren und die erfolgreiche Datenübertragung zu erhöhen.** Der Algorithumus überprüft zunächst ob Datenverkehr im Netzwerk vorhanden ist.

Die Sicherungsschicht kann in zwei Abschnitte unterteilt werden:

![image](https://user-images.githubusercontent.com/83710723/146955067-5f40b002-283f-445e-baaa-bf296575baa8.png)

<br/>

<br/>

<a name="04.1"></a>
### Logical Link Control (LLC)
Die Logical Link Control (LLC) erstellt Pfade für Daten auf dem Ethernet, um zwischen Geräten zu übertragen.

&uarr; [zurück zum Seitenanfang](#top)


<br/>

<br/>

<a name="04.2"></a>
### Meadia Access Controll (MAC)
Die Meadia Access Controll (MAC) verwendet Hardwareadressdaten, die Netzwerkschnittstellenkarten (NIC) zugewiesen sind, um einen bestimmten Comuputer oder ein bestimmtes Gerät zu identifizieren und die Quelle und das Ziel von Datenübertragungen anzuzeigen.

&uarr; [zurück zum Seitenanfang](#top)

<br/>
