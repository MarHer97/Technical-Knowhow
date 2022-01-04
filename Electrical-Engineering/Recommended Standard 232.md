

<a name="top"></a>
# Recommended Standard 232

<br/>

Inhalt des Markdowns `Recommended Standard 232`

**[01 Definition](#01)** <br/>
**[02 ANSI-Norm](#02)** <br/>
**[03 Funktionsweise](#03)** <br/>

<br/>

<br/>

<br/>

<a name="01"></a>
## 01 Definition
**RS-232 (Recommended Standard 232) ist ein [Standard](https://de.wikipedia.org/wiki/Standard) für eine [serielle Schnittstelle](https://de.wikipedia.org/wiki/Serielle_Schnittstelle), der in den frühen 1960er Jahren vom US-amerikanischen Standardisierungsgremium [Electronic Industries Association (EIA)](https://de.wikipedia.org/wiki/Electronic_Industries_Alliance) erarbeitet wurde und bis in die 2010er Jahre häufig bei [Computern](https://de.wikipedia.org/wiki/Computer) vorhanden war.**

<br/>

<br/>

<a name="Verwendung"></a>
### Aktuelle Verwendung
**Weltweit werden immer weniger Geräte mit RS-232-Schnittstelle produziert.** Beispiele sind Service- und Konfigurationsanschlüsse bei Geräten wie z. B. Router, Switches, Speichersysteme, Laborgeräte und Point-Of-Sale-Terminals. Alternative serielle Schnittstellen bieten zuverlässigere und schnellere Verbindungsmöglichkeiten. 

**Nur noch wenige PCs werden mit einem COM-Port ausgeliefert, Notebookhersteller bieten diese Ausstattungsoption nahezu gar nicht mehr an.** Um Geräte, die eine RS-232-Schnittstelle besitzen, mit Computern ohne diese betreiben und programmieren zu können, gibt es Konverter von [USB](https://de.wikipedia.org/wiki/Universal_Serial_Bus) auf RS-232. Auch Steckkarten mit RS-232-Schnittstellen für PCs werden angeboten.

**Viele aktuelle Geräte mit RS-232 nutzen nur drei Adern bzw. Pins (RX, TX, GND), verzichten also auf die Handshake- und Steuerleitungen.** Wegen der niedrigen Datenrate, der vergleichsweise geringen Anforderungen an die Verkabelung und des hohen, toleranten Signalpegels ist die RS-232 auch weiterhin verbreitet, wenn es um Störsicherheit und lange Signalverbindungen geht. **Sie wird jedoch in dieser Hinsicht von Twisted-pair-Netzwerkkabelverbindungen mit Transformator („Ethernet“) sowie vom [RS-485-Standard](https://de.wikipedia.org/wiki/EIA-485) übertroffen.**

Zur Potentialtrennung sowie zur Erhöhung der Störsicherheit werden optische Zwischenstecker angeboten, die ihre Betriebsspannung aus den Signalpegeln beziehen, also keine eigene Stromversorgung benötigen.

Obwohl es zahllose andere serielle Schnittstellenarten gibt, wird die RS-232 traditionell „serielle Schnittstelle“ genannt, weil sie früher speziell im PC-Bereich die einzig übliche war.

&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<br/>

<a name="02"></a>
## 02 ANSI-Norm
**Die aktuelle amerikanische Version heißt offiziell (ANSI EIA/) TIA-232-F und ist aus dem Jahr 1997. Die in den USA und Europa übliche Bezeichnung ist RS-232 (RS steht dabei für Recommended Standard).** Zur Frage der korrekten Bezeichnung siehe den Abschnitt Kennzeichnung von Standards bei [EIA – Electronic Industries Alliance](https://de.wikipedia.org/wiki/Electronic_Industries_Alliance#Standards).

Die EIA hat eine Vielzahl von wichtigen Standards und Normen hervorgebracht, z. B. [RS-232](https://de.wikipedia.org/wiki/RS-232) als Standard für Modemverbindungen weltweit und [EIA-422](https://de.wikipedia.org/wiki/EIA-422) (ehemals RS-422), [RS-423](https://de.wikipedia.org/wiki/EIA-423) und [EIA-485](https://de.wikipedia.org/wiki/EIA-485) (früher RS-485).

&uarr; [zurück zur Übersicht](#top)

<br/>

<br/>

<br/>

<a name="03"></a>
## 03 Funktionsweise
**RS-232 definiert die Verbindung zwischen dem Terminal (Datenendeinrichtung (DEE), engl. data terminal equipment (DTE)) und dem Modem (Datenübertragungseinrichtung (DÜE), engl. data communication equipment (DCE)), was Timing und Spannungspegel betrifft.** Als Steckverbinder wurden die 25-polige D-Sub empfohlen (nicht vorgeschrieben). Das Übertragungsprotokoll ist nicht Bestandteil des Standards. Allgemein sind die Parameter unter Serielle Datenübertragung erläutert.

<br/>

<br/>

<a name="Übertragung"></a>
### Übertragung
**Die Übertragung erfolgt in Wörtern. Ein Wort entspricht dabei je nach Konfiguration fünf bis neun Bits, in dem dann ein einzelnes Zeichen kodiert ist. Meistens erfolgt die Kodierung gemäß [American Standard Code for Information Interchange (ASCII)](https://de.wikipedia.org/wiki/American_Standard_Code_for_Information_Interchange).** 

Häufig kommen auch (ASCII-)Steuercodes für die Ansteuerung eines Terminals wie VT100 zum Einsatz, diese sind im RS-232-Standard jedoch nicht definiert. Üblich ist daher, sieben bzw. acht Datenbits zu übertragen. Jedoch ist beispielsweise auch (nach Anpassung der Signalpegel) die Verarbeitung des 5-bit-Fernschreib-Codes möglich.

&uarr; [zurück zur Übersicht](#top)

<br/>

<br/>

<a name="Serielle"></a>
### Serielle Datenübertragung
**Eine RS-232-Verbindung arbeitet [(bit-)seriell](https://de.wikipedia.org/wiki/Serielle_Daten%C3%BCbertragung) mit je einer Datenleitung für beide Übertragungsrichtungen. Das heißt, die [Bits](https://de.wikipedia.org/wiki/Bit) werden nacheinander auf einer Leitung übertragen, im Gegensatz zur [parallelen Datenübertragung](https://de.wikipedia.org/wiki/Parallele_Schnittstelle).** Die dafür nötige Seriell-Parallel-Wandlung geschieht meistens in sog. [UARTs](https://de.wikipedia.org/wiki/Universal_Asynchronous_Receiver_Transmitter) (entweder als integriertes Modul in einem Mikrocontroller oder als Einzelbaustein).

&uarr; [zurück zur Übersicht](#top)

<br/>

<br/>

<a name="Asynchrone"></a>
### Asynchrone Datenübertragung
**Die Datenübertragung erfolgt [asynchron](https://de.wikipedia.org/wiki/Asynchrone_Daten%C3%BCbertragung), es existiert also kein gemeinsamer Takt. Jeder Teilnehmer kann bei freier Leitung, zu jedem beliebigen Zeitpunkt, vollständige Datenwörter übertragen.** Die Synchronisation in der Übertragung erfolgt durch den Empfänger als sogenannte Wortsynchronisation, also am Anfang durch die Signalflanke des Startbits.

Die Synchronisation des Empfängers geschieht mit dem Start der Übertragung auf der Datenleitung, da das [Stopp-Bit](https://de.wikipedia.org/wiki/Stoppbit) bzw. der Ruhezustand auf der Leitung den inversen Pegel zum Start-Bit aufweist. Der Empfänger synchronisiert sich so in die Mitte der einzelnen Datenbits und tastet die folgenden Bits des Datenwortes mit seiner eigenen [Bitrate](https://de.wikipedia.org/wiki/Bitrate) ab.

Damit das funktioniert, dürfen die Bitraten von Sender und Empfänger nur einige Prozent voneinander abweichen. Jedes übertragene Wort muss somit von einem Startbit (logischer Wert 0) eingeleitet und mit mindestens einem Stopp-Bit (logischer Wert 1) abgeschlossen werden. Das Stopp-Bit ist kein Bit im eigentlichen Sinne, sondern bezeichnet die Mindestlänge der Pause bzw. des Ruhezustands. Daher können zwischen zwei Wörtern beliebig viele Stopp-Bits vorliegen, auch nichtganzzahlige Werte wie 1,5 Stopp-Bits. Damit ist gemeint, dass die Mindestdauer der Pause der Zeitdauer von 1,5 Bitzellen entspricht. Der Grund liegt darin, dass manche UARTs zwischen dem Empfang zweier Wörter eine etwas längere Pause von mehr als einer Bitdauer benötigen.

Zwischen Start- und Stopp-Bit(s) werden die eigentlichen Nutzdaten (Datenbits) über die Taktzeit unverändert (NRZ-codiert) übertragen.

&uarr; [zurück zur Übersicht](#top)

<br/>

<br/>

<a name="Spannungsschnittstelle"></a>
### Spannungsschnittstelle

**RS-232 ist eine Spannungsschnittstelle (im Gegensatz z. B. zu einer [Stromschnittstelle](https://de.wikipedia.org/wiki/Stromschnittstelle)). Die binären Zustände werden durch verschiedene elektrische Spannungspegel realisiert.**

Für die Datenleitungen (TxD und RxD) wird eine negative Logik verwendet, wobei eine Spannung zwischen −3 V und −15 V (ANSI/EIA/TIA-232-F-1997) eine logische Eins und eine Spannung zwischen +3 V und +15 V eine logische Null darstellt. Signalpegel zwischen −3 V und +3 V gelten als undefiniert.

Bei den Steuerleitungen (DCD, DTR, DSR, RTS, CTS und RI) wird der aktive Zustand durch eine Spannung zwischen +3 V und +15 V dargestellt, der inaktive Zustand durch eine Spannung zwischen −3 V und −15 V. Zu beachten ist jedoch, dass die hier angegebenen (und mehrheitlich benutzten) Bezeichnungen für die Steuerleitungen im Original-Standard so nicht vorkommen. Dort sind lediglich gewisse Schaltungen beschrieben, die diesen Bezeichnungen zwar zugeordnet werden können, im Standard aber anders benannt sind.

Die oben angegebenen Spannungen beziehen sich auf die Empfänger (Eingänge). Bei den Sendern (Ausgänge) muss die Spannung mindestens +5 V bzw. −5 V an einer Last von 3 bis 7 kΩ betragen, um genügend Störabstand zu gewährleisten. Üblich ist die Verwendung von +12 V und −12 V.

![image](https://user-images.githubusercontent.com/83710723/148072033-3e51ee78-d119-4642-9756-54671c6a99df.png)

&uarr; [zurück zur Übersicht](#top)

<br/>

<br/>

<a name="Steckverbindung"></a>
### Steckverbindung
**Als Steckverbindung wurden nach der ursprünglichen Norm 25-polige [D-Sub-Stecker](https://de.wikipedia.org/wiki/D-Sub) für DTE und -Buchsen für DCE benutzt.** Da viele der 25 Leitungen reine Drucker- bzw. Terminal-Steuerleitungen aus der elektromechanischen Ära sind, die für die meisten Verbindungen mit moderneren Peripheriegeräten nicht benötigt werden, haben sich heute 9-polige D-Sub-Stecker und -Buchsen etabliert, welche häufig DB-9 genannt werden oder korrekter DE-9. 

Diese waren beim IBM PC/AT ursprünglich als reine Notlösung zum Platzsparen eingeführt worden (damals ging es darum, den Stecker zusammen mit einer ebenfalls verkleinerten Centronics-Schnittstelle auf einer Steckkarte unterzubringen ). Der 9-polige Stecker ist daher auch nicht in der RS-232-Norm zu finden, sondern im Standard EIA/TIA-574. Für die RS-232-Datenübertragung werden selten auch noch andere Konnektoren benutzt, wie z. B. Mini-DIN, Modular 8P8C (unkorrekterweise oft als RJ-45 bezeichnet, spezifiziert in EIA/TIA 561) oder komplett firmenspezifische.

&uarr; [zurück zur Übersicht](#top)

<br/>

<br/>

<a name="Handshake"></a>
### Handshake
**Zur Vermeidung von Datenverlusten muss der Empfänger die Datenübertragung anhalten können, wenn keine weiteren Daten mehr verarbeitet werden können. Dieser sogenannte [Handshake](https://de.wikipedia.org/wiki/Datenflusssteuerung) kann auf zwei Arten realisiert werden, entweder softwareseitig über bestimmte Steuercodes oder über spezielle Leitungen (Hardware-Handshake).**

- Beim Software-Handshake sendet der Empfänger zur Steuerung des Datenflusses spezielle Zeichen an den Sender. Entsprechend werden für die Datenübertragung lediglich drei Leitungen (RxD, TxD und GND) benötigt. Diese Art Handshake ist aber nur möglich, wenn die beiden Steuercodes in den Nutzdaten nicht vorkommen. Beim meist verwendeten Xon/Xoff-Protokoll sendet der Empfänger zur Steuerung des Datenflusses spezielle Zeichen an den Sender (Xon = 11h und Xoff = 13h).
- Beim Hardware-Handshake signalisieren sich die beiden Geräte über zusätzliche Steuer- und Meldeleitungen ihren jeweiligen Status. Ein Minimal-Interface mit Hardware-Handshake besteht beispielsweise aus fünf Leitungen (TxD, RxD, GND, RTS und CTS).

&uarr; [zurück zur Übersicht](#top)

<br/>

<br/>

<a name="Leitungslänge"></a>
### Leitungslänge und Übertragungsrate
**Da die Signalqualität mit zunehmender Leitungslänge abnimmt, ist die Leitungslänge begrenzt.**

Ein begrenzender Faktor ist die Laufzeit des Signals. Da eine RS-232-Schnittstelle am Leitungsende nicht mit ihrem Wellenwiderstand abgeschlossen werden kann (zu große Verlustleistung), gibt es unweigerlich Leitungsreflexionen. Mit zunehmender Übertragungsrate und Kabellänge stören die Reflexionen immer mehr die Datenübertragung. Die Norm verlangt, dass die Flankensteilheit am Sender den Wert 30 V/µs nicht überschreiten darf, womit die Auswirkungen der Reflexionen begrenzt werden. Empfängerseitig wird durch einen Schmitt-Trigger wieder ein Rechtecksignal mit sehr hoher Flankensteilheit hergestellt.

Ein weiterer Aspekt ist, dass die Signalübertragung nicht differentiell, sondern asymmetrisch (single-ended bzw. unbalanced) erfolgt. Das zu übertragende Signal beinhaltet einen Gleichspannungsanteil und ist deshalb relativ empfindlich auf Gleichtaktstörungen. Solche Störungen können z. B. durch induktive Einkopplung in die Schleife RxD-GND entstehen. Weil sich alle Signale auf das gleiche GND-Signal beziehen, kann ein Strom auf der TxD-Leitung einen Spannungsabfall auf der GND-Leitung erzeugen, welcher zu einer Potentialverschiebung zwischen den beiden Kommunikationspartnern führt und beispielsweise auf der RxD-Leitung gesehen wird und Störungen verursacht.

Laut ursprünglichem Standard ist eine Kabelkapazität von max. 2500 pF zulässig, was bei Standardkabeln einer Kabellänge von max. 15 m (50 Fuß) entspricht. Mit Kabeln, welche eine besonders niedrige Kapazität aufweisen (beispielsweise UTP CAT-5 Kabel mit 55 pF/m), lassen sich konform zur Definition 45 m erreichen. Die nebenstehende Tabelle gibt Erfahrungswerte von Texas Instruments wieder.

Die Probleme der gegenseitigen Beeinflussung über GND, fehlender Abschlusswiderstand etc. lassen sich durch eine differentielle Übertragung wie bei RS-485, LVDS etc. beheben.

<br/>

**Maximalwerte für die [Baudrate](https://de.wikipedia.org/wiki/Baud) und Leitungslänge**

| Datenrate (kBd) | Länge (m) | 
|---|---|
| 2,4 | 900 |
| 4,8	 | 300  |
| 9,6 | 152|
| 19,2 | 15 |
| 57,6 | 5 |
| 115,2	 | < 2 |

&uarr; [zurück zur Übersicht](#top)

<br/>

<br/>

<a name="Verkabelung"></a>
### Verkabelung und Stecker
**Um zwei Geräte über die serielle Schnittstelle zu verbinden, müssen die „hörenden“ Leitungen des einen Gerätes mit den „sprechenden“ der anderen Seite verbunden werden.** Bei Terminals bzw. Rechnern (DTE– data terminal equipment) sind „sprechende“ Leitungen TxD, RTS und DTR, „hörende“ Leitungen sind RxD, CTS, DSR, DCD und RI. Bei Modems (DCE– data circuit-terminating equipment) ist es genau umgekehrt; es gibt die vom Terminal „gesprochenen“ Signale an die Gegenseite weiter und muss daher auf diese „hören“, andersherum werden die von der Gegenseite „gehörten“ Signale zum Terminal „weitergesagt“.

![image](https://user-images.githubusercontent.com/83710723/148074192-addc847a-62fd-44db-ba51-d8d191c8d0c4.png)
![image](https://user-images.githubusercontent.com/83710723/148074225-1761d187-afcd-4488-a7b7-c8787274d5a3.png)

<br/>

**Pinbelegung**

| Abkürzung     | Name                  | Beschreibung                                                                                                                                                                                                                                                                                                                          | Pin-Nr.<br>DB-25 | Pin-Nr.<br>DE-9 | Pin-Nr.<br>[Modular 8P8C](https://de.wikipedia.org/wiki/RJ-Steckverbindung "RJ-Steckverbindung") | Richtung beim DTE (z. B. PC) | Richtung beim DCE (z. B. Modem) |
| ------------- | --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- | --------------- | ------------------------------------------------------------------------------------------------ | ---------------------------- | ------------------------------- |
|               | Common Ground         | Gemeinsame Abschir[mmasse](https://de.wikipedia.org/wiki/Masse_(Elektronik) "Masse (Elektronik)") (nicht Datenmasse)                                                                                                                                                                                                                  | 1                | —               | —                                                                                                | —                            | —                               |
| CTS           | Clear to Send         | „Sendeerlaubnis“; Ein High-Pegel an diesem Eingang ist ein Signal der Gegenstelle, dass sie Daten von DTE entgegennehmen kann                                                                                                                                                                                                         | 5                | 8               | 7                                                                                                | Eingang                      | Ausgang                         |
| DCD, CD, RLSD | (Data) Carrier Detect | Mit einem High-Pegel an diesem Eingang signalisiert die Gegenstelle, dass sie einlaufende Daten auf der Leitung erkennt (dem Namen nach ist das die [Modulationsträger](https://de.wikipedia.org/wiki/Tr%C3%A4ger_(Nachrichtentechnik) "Träger (Nachrichtentechnik)")\-Erkennung) und an DTE weitergeben möchte                       | 8                | 1               | 2                                                                                                | Eingang                      | Ausgang                         |
| DSR           | Data Set Ready        | Ein High-Pegel an diesem Eingang ist ein Signal der Gegenstelle, dass sie im Prinzip einsatzbereit ist (aber nicht notwendigerweise auch empfangsbereit, siehe CTS)                                                                                                                                                                   | 6                | 6               | 1                                                                                                | Eingang                      | Ausgang                         |
| DTR           | Data Terminal Ready   | Mit einem High-Pegel an diesem Ausgang signalisiert DTE seine Betriebsbereitschaft an die Gegenstelle. Damit kann die Gegenstelle, z. B. ein Modem, aktiviert oder auch zurückgesetzt werden. Üblicherweise antwortet die Gegenstelle mit einem High-Pegel auf DSR                                                                    | 20               | 4               | 3                                                                                                | Ausgang                      | Eingang                         |
| GND           | Ground                | Signalmasse. Die Signalspannungen werden gegen diese Leitung gemessen.                                                                                                                                                                                                                                                                | 7                | 5               | 4                                                                                                | —                            | —                               |
| RI            | Ring Indicator        | Ein High-Pegel an diesem Eingang signalisiert dem DTE-Gerät, dass ein Anruf ankommt, d. h., dass jemand eine Datenverbindung aufbauen will („ring“ ist engl. für „klingeln“; besonders bei Telefonen und im übertragenen Sinne auch bei Modems). Siehe auch _[Rufspannung](https://de.wikipedia.org/wiki/Rufspannung "Rufspannung")_. | 22               | 9               | —                                                                                                | Eingang                      | Ausgang                         |
| RTR           | Ready to Receive      | „Empfangsstatus“; ein [High-Pegel](https://de.wikipedia.org/wiki/Logikpegel "Logikpegel") an diesem Ausgang signalisiert der Gegenstelle, dass DTE bereit ist, Daten zu empfangen                                                                                                                                                     | 4                | 7               | 8                                                                                                | Ausgang                      | Eingang                         |
| RTS           | Request to Send       | „Sendeanforderung“; ein [High-Pegel](https://de.wikipedia.org/wiki/Logikpegel "Logikpegel") an diesem Ausgang signalisiert, dass DTE Daten senden möchte                                                                                                                                                                              | 4                | 7               | 8                                                                                                | Ausgang                      | Eingang                         |
| RxD, RX, RD   | Receive Data          | Leitung für eingehende (von DTE zu empfangende) Daten (negative Logik).                                                                                                                                                                                                                                                               | 3                | 2               | 5                                                                                                | Eingang                      | Ausgang                         |
| TxD, TX, TD   | Transmit Data         | Leitung für ausgehende (von DTE gesendete) Daten ([negative Logik](https://de.wikipedia.org/wiki/Negative_Logik "Negative Logik")).                                                                                                                                                                                                   | 2                | 3               | 6                                                                                                | Ausgang                      | Eingang                         |

&uarr; [zurück zur Übersicht](#top)

<br/>

<br/>
