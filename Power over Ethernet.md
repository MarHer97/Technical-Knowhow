<a name="top"></a>
# Power over Ethernet

<br/>

Inhalt des Markdowns Power over Ethernet

**[01 Definition](#01)** <br/>
**[02 Vorteile](#02)** <br/>
**[03 Voraussetzungen](#03)** <br/>
**[04 Standards](#04)** <br/>



<br/>

<br/>

<br/>

<a name="01"></a>
## 01 Definition
**Die Stromversorgung über Ethernet, englisch Power over Ethernet (PoE), bezeichnet Verfahren, mit dem netzwerkfähige Geräte über das achtadrige Ethernet-Kabel mit Strom versorgt werden können.** Neben den durch IEEE 802.3 standardisierten, jeweils abwärtskompatiblen Varianten existieren einige proprietäre Verfahren sowie einfache, passive Varianten.

PoE wird von Netzwerkgeräten genutzt, die wenig Leistung benötigen. Es wird typischerweise in IP-Telefonen, kleinen Hubs, Kameras, kleinen Servern oder in schnurlosen Übertragungsgeräten, wie WLAN-Zugangspunkten oder Bluetooth-Geräten eingesetzt.

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
