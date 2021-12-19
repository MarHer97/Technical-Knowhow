<a name="top"></a>
# Power over Ethernet

<br/>

Inhalt des Markdowns Power over Ethernet

**[01 Definition](#01)** <br/>
**[02 Vorteile](#02)** <br/>
**[03 Herausforderungen](#03)** <br/>
**[04 IEEE-Spezifikationen](#04)** <br/>



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
## 03 Herausforderungen
**Die höhere Stromstärke stellt die Datenverkabelung vor neue Herausforderungen: Wo mehr Strom fließt, wird durch den Widerstand mehr Wärme erzeugt. Wärmere Kabel dämpfen die Datenübertragung mehr als zuvor. Das kann dazu führen, dass nicht mehr genug Signal zum Empfänger gelangt und die Datenübertragung unmöglich wird.** Bei der Planung einer neuen, PoE-tauglichen LAN-Verkabelung muss dieser Effekt berücksichtigt werden. Die maximale Übertragungslänge muss den Temperaturbedingungen angepasst und verkürzt werden.

&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<br/>

<a name="04"></a>
## 04 IEEE-Spezifikationen
Im engeren Sinne wird heute mit PoE einer der IEEE-Standards 802.3 gemeint. Zuerst wurde im Juni 2003 Clause 33 „DTE Power over MDI“ in IEEE 802.3af-2003 mit bis zu 12,95 W am Gerät verabschiedet. Dieser wurde zuerst durch IEEE 802.3at-2009[3] leistungsmäßig erweitert – vor der Standardisierung auch als PoE+ oder PoE plus bekannt –, der die maximale Leistungsabgabe auf 25,5 W erhöhte. Schließlich folgte IEEE 802.3bt-2018 Clause 145 „Power over Ethernet“ (auch 4PPoE) mit nunmehr bis zu 71,3 Watt, der gleichzeitigen Übertragung von Energie über alle vier Leitungspaare und der Erweiterung auf 2.5GBASE-T, 5GBASE-T und 10GBASE-T.

<br/>

**Vergleich der PoE-Standards:**

| IEEE-Standard                       | PoE (802.3af-2003) | PoE Plus (802.3at-2009) | 4-paar PoE (802.3bt-2018) |
| :---------------------------------- | :----------------- | :---------------------- | :------------------------ |
| Ausgangsspannung in V (DC)          | 36–57              | 42,5–57                 | 42,5–57                   |
| Ausgangsstrom Betrieb in mA (DC)    | 350                | 600                     | 2× 960                    |
| Ausgangsstrom Startmodus in mA (DC) | 400                | 400                     | ?                         |
| Leistung der (PSE)-Versorgung in W  | max. 15,4          | max. 30                 | 45; 60; 75; 90            |
| Leistung am Endgerät (PD) in W      | max. 12,95         | max. 25,5               | 40; 51; 62; 71            |
| PSE-Klasse                          | 1; 2; 3            | 4                       | 5; 6; 7; 8                |
| unterstützte Endgeräte (PD-Type)    | 1                  | 1 und 2                 | 1; 2; 3; 4                |
| Benutzte Adernpaare                 | 2                  | 2                       | 2 und 4                   |

&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<br/>
