

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

<br/>

**Vorteile digitaler Übertragung**

Benötigt eine Informationen mehr Bandbreite als zur Verfügung steht, dann wird die Information nicht einfach abgeschnitten, sondern zwischengespeichert und nacheinander übertragen. Das geht bei analogen Signalen nicht.

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
**Parallele Datenübertragungen übertragen digitale Daten über mehrere Leitungen gleichzeitig. Die Übertragung erfolgt dabei auf mehreren physischen Leitungen nebeneinander oder über mehrere Kanäle zur gleichen Zeit im "Gleichschritt".** Werden nur binäre Symbole mit zwei möglichen Zuständen eingesetzt, entspricht ein Symbol einem Bit, welches pro Datenpfad übertragen werden kann. Bei n parallelen Datenpfaden können n Bits in einem Schritt parallel übertragen werden.

Die parallele Übertragung über mehrere serielle Datenkanäle unterscheidet sich grundlegend von einer parallelen Datenübertragung in der Weise, dass dort auf der unteren Hardwareebene alle Kanäle unabhängig voneinander übertragen und Laufzeitunterschiede irrelevant sind. Bei parallelen Übertragungen arbeiten alle Datenkanäle streng mit einem gemeinsamen Taktregime und sind dadurch sehr empfindlich auf Laufzeitunterschiede der Kanäle.

<br/>

**Nachteile der Parallelen Datenübertragung**

Der wesentliche Nachteil der parallelen Datenübertragung, neben dem Umstand, eine Vielzahl von parallelen Datenübertragungspfaden zu benötigen, ist der Umstand, dass die einzelnen Laufzeiten entlang der parallelen Leitungen nicht alle exakt gleich sind. Diese Ungleichheiten können beispielsweise durch kleine Abweichung in den Leitungslängen und anderen Toleranzen im physikalischen Aufbau der Übertragungsstrecke bedingt sein. Dadurch kommt es, insbesondere bei höheren Schrittgeschwindigkeiten, zu Empfangsfehlern bzw. einer Beschränkung der Schrittgeschwindigkeit und damit der Datenübertragungsrate. Aus diesem Grund werden bei höheren Übertragungsraten serielle Übertragungsverfahren eingesetzt, auch wenn durch die serielle Aneinanderreihung der einzelnen Symbole hohe Symbolraten und große Bandbreiten die Folge sind.

&uarr; [zurück zum Seitenanfang](#top)


<br/>

<br/>

Weiterführende Literatur:
- [Datenübertragung, Website Elektronik Kompendium](https://www.elektronik-kompendium.de/sites/kom/0212091.htm)
- [Übertragungstechnik, Website Elektronik Kompendium](https://www.elektronik-kompendium.de/sites/kom/1303291.htm)
- [Übertragungstechnik Grundbegrriffe, Website Elektronik Kompendium](https://www.elektronik-kompendium.de/sites/kom/1607151.htm)




<br/>
