

<a name="top"></a>
# Datenübertragung

<br/>

Inhalt des Markdowns Datenübertragung

**[01 Definition](#01)** <br/>
> [Analoge und Digitale Übertragungstechnik](#Übertragungstechnik) <br/>

**[02 Analoge Informationsübertragung](#02)** <br/>
**[03 Digitale Informationsübertragung](#03)** <br/>
> [Serielle Datenübertragung](#seriell) <br/>
> [Parallele Datenübertragung](#parallel) <br/>

**[04 Standards](#04)** <br/>



<br/>

<br/>

<br/>

<a name="01"></a>
## 01 Definition
**Mit Datenübertragung oder Informationsübertragung bezeichnet man grundsätzlich alle Methoden, die (Nutz-)Informationen von einem Sender (Informationsquelle) zu einem Empfänger (Informationssenke) übermitteln.**

Speziell auf der technischen Ebene – und hier insbesondere in der Kommunikationstechnik und (als deren Teilgebiet) der Nachrichtentechnik – wird dazu vom Sender eine physikalische Größe (bspw. elektrische Spannung oder die Frequenz von elektromagnetischen Wellen) zeitlich variiert und dies dann vom Empfänger gemessen.
In der Übertragungstechnik unterscheidet man zwischen der Information und dem Signal. Die Information bezeichnet das, was übertragen wird. Das Signal definiert, wie es übertragen wird. Sowohl Information als auch das Signal können analog oder digital sein.

<br/>

<br/>

<a name="Übertragungstechnik"></a>
### Analoge und Digitale Übertragungstechnik

**In der Übertragungstechnik unterscheidet man zwischen der Information und dem Signal. Die Information bezeichnet das, was übertragen wird. Das Signal definiert, wie es übertragen wird. Sowohl Information als auch das Signal können analog oder digital sein.**

Ein analoges Signal ist eine physikalische Größe (bspw. elektrische Spannung oder die Frequenz von elektromagnetischen Wellen), die im Verlauf der Größe (Amplitude) als auch im zeitlichen Verlauf kontinuierliche Werte annehmen kann. Ein digitales Signal ist eine physikalische Größe, die nur bestimmte diskrete Werte annehmen kann. Die Werte entsprechen der Anzahl der vereinbarten Zustände. Werden zwei Zustände vereinbart, dann handelt es sich um binäre (digitale) Signale. Analoge Signale bestehen aus einem kontinuierlichen Signal- bzw. Datenstrom. Den gibt es bei digitalen Signalen nicht. 

![image](https://user-images.githubusercontent.com/83710723/147656547-805d0374-2d5a-447a-b8dd-ae250a429c4f.png)

**Man unterscheidet zwischen analogen und digitalen Signalen bzw. analogen und digitalen Informationen. Insgesamt gibt es 4 verschiedene Signal- und Informations-Kombinationen:**
- [Analoge Information - Analoges Signal (Direkt)](#Direkt)
- [Digitale Information - Analoges Signal (Modem)](#Modem)
- [Digitale Information - Digitales Signal (Interface)](#Interface)
- [Analoge Informationen digital übertragen (Codec)](#Codec)

<br/>

<br/>

<a name="Direkt"></a>
#### Analoge Information - Analoges Signal (Direkt)
Soll eine analoge Information analog übertragen werden, dann ist das relativ einfach. Es ist kein spezielles Interface notwendig. Zwar gibt es auch hier bestimmte Schnittstellen und Verarbeitungselemente, doch deren Funktion ist relativ einfach. Im Prinzip ist das so, wie wenn man einen Lautsprecher an einen Audio-Verstärker anschließt. Das Signal wird über ein Kabel vom Verstärker zum Lautsprecher geführt. Und der Lautsprecher gibt das Signal als Schall aus.

&uarr; [zurück zum Seitenanfang](#top)

<br/>

<a name="Modem"></a>
#### Digitale Information - Analoges Signal (Modem)
Schwieriger wird es, wenn eine digitale Information analog übertragen werden soll. Typischer Fall ist der Einsatz eines Modems, dass die digitalen Daten aus einem Computersystem in analoge Signale umwandelt, um sie über das Telefonnetz zu übertragen.
Modem ist ein Kunstwort. Es besteht aus den Begriffen Modulator und Demodulator.

&uarr; [zurück zum Seitenanfang](#top)

<br/>

<a name="Interface"></a>
#### Digitale Information - Digitales Signal (Interface)
Leicht anzunehmen wäre es, dass sich digitale Informationen ohne Probleme digital übertragen lassen würden. Doch weit gefehlt. Digitale Signale haben den Nachteil, dass sie sehr störanfällig sind. Vor der Übertragung müssen digitale Signale für die Übertragung aufwändig aufbereitet werden.

&uarr; [zurück zum Seitenanfang](#top)

<br/>

<a name="Codec"></a>
#### Analoge Informationen digital übertragen (Codec)
Wenn analoge Informationen in digitale Signale umgewandelt werden müssen, dann ist dafür ein Codec verantwortlich. Es handelt sich um ein Kunstwort, bestehend aus Coder und Decoder. Das analoge Signal wird in ein digitales Signal codiert und umgekehrt decodiert. Bei der Codierung bekommt ein analoger Wert einen digitalen Wert, der dann übertragen wird. Beim Empfänger wird der digitale Wert in den analogen Wert decodiert.

&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<br/>

<a name="02"></a>
## 02 Analoge Informationsübertragung

**Bei der analogen Übertragung von Information werden der physikalischen Größe die entsprechenden Daten kontinuierlich aufgeprägt. Jeder Wert ist dabei in einem festgelegten Intervall zulässig und zu jedem Zeitpunkt relevant.**

Die technische Unmöglichkeit den Nachrichtenkanal (das heißt die physikalische Größe) so gut von der Außenwelt abzuschirmen, dass dieser nicht von ihr beeinflusst wird, sowie die technische Unmöglichkeit die physikalische Größe exakt zu messen, führen mit der Zeit zum Informationsverlust, der auch nicht durch Verstärker verhindert werden kann.

&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<br/>

<a name="03"></a>
## 03 Digitale Informationsübertragung
**Um Daten sowohl innerhalb des eigentlichen Rechners als auch an bzw. von Peripheriegeräten zu übertragen benötigt man Schnittstellen (Interfaces). Je nach den Anforderungen können diese sowohl das Übertragungsverfahren betreffend als auch in ihren technischen Spezifikationen sehr unterschiedlich sein.** Auch die Konventionen wie Daten zwischen Sender und Empfänger zu übermitteln sind (Übertragungsprotokoll) können selbst bei physischer Ähnlichkeit der Schnittstelle sehr verschieden sein.

Als Übertragungsverfahren ist die elektrische Signalübertragung zweier (digitaler) Werte (Zustände) sowohl drahtgebunden als auch drahtlos über Funkstrecken weitverbreitet. Dazu kommt noch die aufgrund ihrer vielen Vorteile optische Datenübertragung mittels Glas- oder Kunststoffasern. Letztgenanntes Verfahren ist in der Industrie wegen der Störsicherheit, im kommerziellen Bereich wegen des hohen Datentransfervolumens und bei militärischen Anwendungen wegen der großen Abhörsicherheit weitverbreitet.

**Grundsätzlich kann man alle Schnittstellen in zwei Kategorien der Datenübertragung einteilen: (1) die einzelnen Digitalwerte werden zeitlich hintereinander übertragen ([serielle Datenübertragung](#seriell)) oder (2) Gruppen von Digitalwerten (Bytes) werden zur gleichen Zeit übertragen ([parallele Datenübertragung](#parallel)).**

![image](https://user-images.githubusercontent.com/83710723/147655775-6c749ab1-511c-4d38-83d2-5894c4db3bc9.png)


Bekannte serielle Schnittstellen sind der USB-Bus, RS-232 und Netzwerkschnittstellen. Parallele Schnittstellen sind etwa der PCI Bus (in ihrem PC), Druckerschnittstelle (sofern dazunicht wie heute bereits verbreitet der USB Bus verwendet wird) und GPIB Bus. Aus diesen Beispielen kann man schon Vor- bzw. Nachteile der beiden Kategorien abschätzen: 
- Über „lange“ Strecken ist die serielle Übertragung insbesondere bei kabelgebundenen Verfahren im Vorteil da minimal nur zwei Leiter (Drähte) benötigt werden,
- dafür ist die mögliche Übertragungsgeschwindigkeit (bei gleichem technischen Aufwand) kleiner als bei parallelen Schnittstellen. Zum Beispiel benötigt der PCI Bus in seiner ursprünglichen Form 32 + 1(Masse) Leitung kann dafür aber bei einer Taktfrequenz von 33 MHz theoretisch etwa 1Gbit/s (1 Bit = 1 digitale Informationseinheit, E/A-Schalter) übertragen. Verwendet man für die serielle Übertragung eine Frequenz von 33
MHz so kommt man rechnerisch zwar auf 33 Mbit/s. 
- Aufgrund des notwendig aufwendigeren Übertragungsprotokolls (Sie müssen Marken zum Kennzeichnen wo eine Dateneinheit beginnt bzw. endet ebenfalls übertragen) reduziert sich dieser Wert.

&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<a name="seriell"></a>
### Serielle Datenübertragung
**Serielle Datenübertragungen übertragen digitale Daten autonom jeweils auf einer Leitung (bzw. auf einem Leitungspaar). Im Gegensatz hierzu werden bei parallelen Datenübertragungen Daten [synchron](#synchron) über mehrere Leitungen übertragen.** Der grundlegende Unterschied ist, dass man bei seriellen Übertragungen keine Laufzeitunterschiede verschiedener Leitungen berücksichtigen muss, was wesentlich höhere Taktfrequenzen erlaubt. 

Der Name seriell assoziiert falsche Vorstellungen, da im Prinzip jede Datenübertragung seriell arbeitet. Ein besserer Name ist bit-serielle Datenübertragung (im Gegensatz zur byte-seriellen Übertragung einer Centronics-Schnittstelle), aber auch dieser Name weckt falsche Assoziationen, da auch bei seriellen Datenübertragungen mehrere Leitungen parallel genutzt werden können (z. B. PCI Express, Gigabit-Ethernet, HDMI) und komplexere Modulationen verwendet werden können, die keine einzelnen Bits mehr kennen (PCI Express, USB 3.0, USB 3.1, SATA, Ethernet ab Fast Ethernet). 

**Für die seriellen Datenübertragungen sind verschiedene serielle Schnittstellen definiert.** Diese umfassen 
- Stecker, 
- Spannungen, 
- Modulationen, 
- verwendete Protokolle sowie 
- Softwareschnittstellen.

Heutzutage kommen bis auf wenige Ausnahmen (DDR-RAM-Anbindung an CPUs sowie Legacy-Schnittstellen) nur noch serielle Datenübertragungen zum Einsatz. Selbst ultraschnelle AD-Wandler benutzen serielle Schnittstellen zur Ausgabe der gewandelten Daten. Früher (bis in die 1990er Jahre) wurden serielle Schnittstellen für langsamere Datenübertragungen (bis ca. 10 KByte/s) über ggf. längere Distanzen (einige hundert Meter) verwendet, parallele Schnittstellen für schnellere Übertragungen (bis 1 MByte/s) über kürzere Entfernungen.

<br/>

**Eigenschaften**
Im Folgenden werden einige Begriffe oder Merkmale aufgezählt, die grundsätzlich jedem seriellen Übertragungsstandard zuzuordnen sind. Des Weiteren wird zwischen Eigenschaften der physikalischen Schnittstelle Hardware und den Protokollen unterschieden.

- Steckeraufbau, Pin-Belegung
- Differentielle (balanced) Übertragung oder nicht-differentielle Übertragung
- Spannungen, Ströme, Impedanzen, Abschlusswiderstände, Wellenlänge (bei optischen Übertragungen)
- Gleichspannungsanteil, galvanische Trennung
- Unidirektional: Simplex, Bidirektional: Halb-Duplex, Voll-Duplex
- Leitungskodierung bzw. Modulation
- Selbsttaktend oder mit zusätzlichem Taktsignal
- Anzahl der Übertragungskanäle, je Richtung
- Hard- oder Software-Handshake
- Übertragungsfehlerbehandlung: Parität, CRC, Hamming-Distanz etc. (siehe Kodierungstheorie)
- Punkt-zu-Punkt-Verbindung (P2P) oder Multipoint (serieller Bus)
- Arbitrierung: Multimaster oder Masterslave
- Echtzeitfähigkeit: z. B. bei Feldbussen erforderlich
- Bei Datenbussen Arbitrierung: Prioritätensteuerung über Token, CSMA etc.

Es gibt verschiedene Standards zu seriellen Schnittstellen, über die eine serielle Übertragung erfolgen kann.

<br/>

<a name="synchron"></a>
#### Synchron

Bei der [synchronen Datenübertragung](https://de.wikipedia.org/wiki/Synchrone_Daten%C3%BCbertragung) werden die Daten in Blocks zusammengefasst und zusammen übertragen. Bei der synchronen Übertragung sind nicht mehr für jedes Datenbyte jeweils einzelne Start-Bits nötig. Die Nutzdaten werden paketorientiert in größeren Blöcken zusammengefasst oder als ein kontinuierlicher Datenstrom übertragen. Die Übertragung wird damit effizienter. Frühe Vertreter dieser Übertragungstechnik waren HDLC und SDLC aus den 1970er Jahren.


&uarr; [zurück zum Seitenanfang](#top)


<br/>

<br/>

<a name="parallel"></a>
### Parallele Datenübertragung


&uarr; [zurück zum Seitenanfang](#top)

<br/>

<br/>

<br/>

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
