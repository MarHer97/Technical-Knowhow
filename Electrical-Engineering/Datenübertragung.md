

<a name="top"></a>
# Datenübertragung

<br/>

Inhalt des Markdowns Datenübertragung

**[01 Definition](#01)** <br/>
**[02 Vorteile](#02)** <br/>
**[03 Voraussetzungen](#03)** <br/>
**[04 Standards](#04)** <br/>



<br/>

<br/>

<br/>

<a name="01"></a>
## 01 Definition
**Die serielle [Schnittstelle](https://de.wikipedia.org/wiki/Schnittstelle) ist eine umgangssprachliche Bezeichnung für eine Schnittstelle zur Datenübertragung zwischen zwei Geräten, bei denen einzelne [Bits](https://de.wikipedia.org/wiki/Bit) zeitlich nacheinander übertragen werden ([Serielle Datenübertragung](https://de.wikipedia.org/wiki/Serielle_Daten%C3%BCbertragung)).** Die Bezeichnung wird in Abgrenzung zu einer [parallelen Schnittstelle](#https://de.wikipedia.org/wiki/Parallele_Schnittstelle) benutzt, bei der mehrere Bits zeitgleich auf mehreren Stromkreisen übertragen werden. Beide Bezeichnungen sind unpräzise und werden für eine große Anzahl unterschiedlicher Schnittstellendefinitionen benutzt.

Gegenüber parallelen Schnittstellen benötigt die serielle Schnittstelle weniger Stromkreise und demzufolge einen geringeren Verkabelungsaufwand, was besonders bei größeren Distanzen bedeutsam ist. Parallele Schnittstellen boten historisch größere Übertragungsgeschwindigkeiten und wurden daher für Anwendungen bevorzugt, bei denen große Datenmengen über kurze Distanz zu übertragen waren, wo die Kabelkosten nicht dominierten. Dieses Argument ist allerdings inzwischen obsolet, die technische Entwicklung der seriellen Schnittstellen hat die der parallelen Schnittstellen überholt.

Im engeren Umfeld von Personal Computern ist mit der seriellen Schnittstelle meist eine Schnittstelle nach EIA-RS-232 gemeint, in der Regel unter Verwendung eines 9-pin D-Sub-Steckers. Sie dient dort traditionell dem Anschluss von Peripheriegeräten an den PC, die mit vergleichsweise moderaten Übertragungsgeschwindigkeiten auskommen, wie z. B. Tastaturen, Mäuse, Drucker, DFÜ-Geräte etc., ist aber inzwischen weitgehend durch die universellere USB-Schnittstelle ersetzt worden. Die USB-Schnittstelle arbeitet zwar ebenfalls seriell, ist aber umgangssprachlich meist nicht gemeint, wenn man von "der seriellen Schnittstelle" redet. Zwischen USB und RS-232 existieren günstige Adapter, so dass die meisten PC-Hersteller dazu übergegangen sind, auf die RS-232 Schnittstelle im Grundgerät zu verzichten.

Serielle Schnittstellen im weiteren Sinn sind sehr weit verbreitet und existieren in sehr vielen Ausprägungen und Varianten. Es gehören dazu neben Punkt-zu-Punkt Verbindungen wie RS-232 und RS-422 auch Netzwerk- und Busschnittstellen, wie z. B. Ethernet, CAN-Bus oder RS-485. Datenraten, mögliche Übertragungsdistanzen und andere Eigenschaften unterscheiden sich z. T. beträchtlich, so existiert für fast jeden Anwendungsbereich eine passende Schnittstellendefinition. Siehe dazu die Auflistung weiter unten.

Serielle Schnittstellen unterscheiden sich nicht nur durch den verwendeten Steckverbinder und die elektrischen Übertragungsparameter, sie benutzen auch unterschiedliche Methoden zur Übertragungssteuerung, Datenflusskontrolle und zur Synchronisation (siehe dazu Kommunikationsprotokoll). Sie können in eine Richtung („simplex“) oder in beide Richtungen („duplex“) arbeiten, Letzteres entweder abwechselnd („halb-duplex“) oder gleichzeitig („voll-duplex“) (siehe dazu Duplex (Nachrichtentechnik)).

&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<br/>

<a name="02"></a>
## 02 Vorteile

**Hauptvorteil von PoE ist, dass man ein Stromversorgungskabel einsparen kann und so auch an schwer zugänglichen Stellen oder in Bereichen, in denen viele Kabel stören würden, Ethernet-angebundene Geräte installieren kann. Zusätzlich kann auch die Steckdose eingespart werden und eine schnelle Inbetriebnahme wird garantiert, ganz ohne lästige Verkabelung.** Die Stromversorgung zum Gerät muss nicht separat mit einem Stromkabel und Netzgerät zugeführt oder mit einer Batterie gelöst werden. Das Gerät bezieht die Energie stattdessen über das Datennetz. Dazu muss – meist an zentraler Stelle, im Netzwerkverteiler – neben den Datensignalen zusätzlich Strom in die Datenleitung eingespeist werden. Somit lassen sich einerseits zum Teil Installationskosten einsparen, andererseits kann der damit einfach zu realisierende Einsatz einer zentralen unterbrechungsfreien Stromversorgung (USV) die Ausfallsicherheit der angeschlossenen Geräte erhöhen.

&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<br/>

<a name="03"></a>
## 03 Voraussetzungen
Damit ein Gerät Strom über das Datennetz beziehen kann, muss neben Daten zusätzlich Strom in die Datenleitung eingespeist werden – idealerweise im Netzwerkverteiler. So eignet sich dieses Verfahren vor allem für IP-Telefone, Switche, WLAN-Access-Points oder Überwachungskameras.

Ein weiterer Punkt, der vor der Installation bedacht werden muss, ist die zusätzliche Erwärmung des Kabels. Je mehr Strom durch das LAN-Kabel fließt, umso mehr Wärme wird durch den Widerstand erzeugt. Dies beeinträchtigt jedoch die Datenübertragung. Deshalb sollte im Vorfeld geklärt werden, welcher Belastung das Kabel standhalten muss und wie die Wärme des Kabels abfließen kann.

Zudem kann das LAN-Kabel nicht beliebig lang sein, denn bei längeren Leitungen kommt es zum Spannungsabfall. Deshalb muss beim Kauf des Kabels schon auf den Aderquerschnitt geachtet werden, der nicht über einem AWG-Wert von 24 liegen sollte (CAT5).

&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<br/>

<a name="04"></a>
## 04 Standards
Der IEEE 802.3af-2003-Standard versorgt Geräte mit bis zu 15,4 W (min. 44 V und 350 mA) auf jedem Port. Jedoch sind nur 12,95 W garantiert, denn ein gewisser Anteil geht bei der Übertragung verloren.

Der neuere IEEE 802.3at-2009-Standard (auch bekannt als PoE+) bietet bis zu 25,5 W. Dieser Standard verbietet die Stromübertragung über alle vier Signalpaare.

Ein weiterer Standard, der vor allem im industriellen Umfeld wie zum Beispiel in Fahrzeugen oder Produktionsmaschinen wichtig ist, ist IEEE 802.3bu (PoDL) für einpaarige Leitungen. Hier gibt es zehn Stufen von 5 bis 50 W.

Eine neue Weiterentwicklung, der IEEE 802.3bt-Standard (4PPoE oder PoE++) soll noch größere Kapazitäten für die Stromversorgung bereitstellen: bis zu 55 W (Level 3) und 100 W (Level 4). Damit müsste jedes Leitungspaar eine Spannung von bis zu 600, beziehungsweise 960 mA aushalten. So könnte ein ganzer Arbeitsplatz mit Rechner, Bildschirm und Telefon über das LAN-Kabel versorgt werden.

<br/>

**Übersicht der [IEEE 802.3 Normenteile](https://de.wikipedia.org/wiki/IEEE_802)**

802.3 – [CSMA/CD](https://de.wikipedia.org/wiki/Carrier_Sense_Multiple_Access/Collision_Detection)
- 802.3af – [Power over Ethernet](https://de.wikipedia.org/wiki/Power_over_Ethernet)
- 802.3at – [Power over Ethernet](https://de.wikipedia.org/wiki/Power_over_Ethernet)
- 802.3az – [Energy Efficient Ethernet](https://de.wikipedia.org/wiki/Energy_Efficient_Ethernet)

<br/>

**Vergleich der PoE-Standards:**

| Standard     | Klasse | Klassifikationsstrom | Max. Speiseleistung (PSE) | Max. Entnahmeleistung (PD) | Ethernet Typ  |
| :-------------- | :------ | :-------------------- | :------------------------- | :-------------------------- | :------------- |
| IEEE 802.3af | 0      | 0-4 mA               | 15,4 W                    | 0,44-12,95 W               | 10/100 Base-T |
| IEEE 802.3af | 1      | 9-12 mA              | 4,0 W                     | 0,44-3,84 W                | 10/100 Base-T |
| IEEE 802.3af | 2      | 17-20 mA             | 7,0 W                     | 3,84-6,49 W                | 10/100 Base-T |
| IEEE 802.3af | 3      | 26-30 mA             | 15,4 W                    | 6,49-12,95 W               | 10/100 Base-T |
| IEEE 802.3at     | 4      | 36-44 mA             | 25,5 W                    | 12,95-21,90 W              | 10/100 Base-T |

&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<br/>
