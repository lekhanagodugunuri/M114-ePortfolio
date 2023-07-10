# M114-ePortfolio

## Inhaltsverzeichnis
- [Tag 1, 16.05.2023](#tag-1-16052023)
- [Tag 2, 23.05.2023](#tag-2-23052023)
- [Tag 3, 30.05.2023](#tag-3-30052023)
- [Tag 4, 06.06.2023](#tag-4-662023)
- [Tag 5, 13.06.2023](#tag-5-13062023)
- [Tag 6, 20.06.2023](#tag-6-2062023)
### Tag 1 [16.05.2023]
-----------
### 1.1 Theorie 

#### Zahlensysteme 

Zahlensysteme und numerische Codes sind grundlegende Konzepte der Mathematik und Informatik, die verwendet werden, um Zahlen darzustellen, zu speichern und zu verarbeiten. In dieser Zusammenfassung werde ich auf Zahlensysteme, insbesondere das Dezimalsystem und das Binärsystem, sowie auf numerische Codes wie den Unsigned-Code und den Signed-Code eingehen.
Numerische Codes dienen dazu, Zahlen in einem bestimmten Format darzustellen. Der Unsigned-Code wird verwendet, um positive Zahlen darzustellen. Er verwendet alle verfügbaren Bits zur Darstellung des Zahlenwerts. Beispielsweise kann ein 8-Bit-Unsigned-Code Werte von 0 bis 255 darstellen. Der Signed-Code hingegen ermöglicht die Darstellung von sowohl positiven als auch negativen Zahlen. Er verwendet das erste Bit, das als Vorzeichenbit bezeichnet wird, um das Vorzeichen der Zahl anzugeben. 

#### Hex Editor  

Ein Hex-Editor ist ein spezielles Programm, das verwendet wird, um den Inhalt und die Struktur von Dateien auf binärer Ebene zu analysieren und zu bearbeiten. Hex-Editoren zeigen den Inhalt einer Datei in hexadezimaler Form an, wobei jedem Byte ein zweistelliger Hexadezimalwert zugeordnet wird. 
Vorteile: 
1. Analyse von Dateiformaten: Hex-Editoren ermöglichen es Entwicklern und Analysten, die Struktur und das Format von Dateien zu untersuchen. Da Dateien auf binärer Ebene gespeichert sind, ist es oft schwierig, den Inhalt mit einem Texteditor oder einem herkömmlichen Programm zu interpretieren. 
2. Datenbearbeitung: Hex-Editoren bieten die Möglichkeit, den Inhalt von Dateien direkt zu bearbeiten. Dies ist besonders hilfreich, wenn es erforderlich ist, bestimmte Werte oder Muster innerhalb einer Datei zu ändern. 
-----------
### 1.2 Aufgaben 
#### Theorie
Zahlensystem
+ Zweiersystem oder Binärsystem bzw. Dualsystem
Basis: 2
Zeichenvorrat: 0, 1

+ Achtersystem oder Oktalsystem
Basis: 8
Zeichenvorrat: 0, 1, 2, 3, 4, 5, 6, 7, 8

+ Zehnersystem oder Dezimalsystem
Basis: 10
Zeichenvorrat: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9

+ Sechzehnersystem oder Hexadezimalsystem (HEX)
Basis: 16
Zeichenvorrat: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A (=10), B (=11), C (=12), D (=13), E (=14), F (=15)

Aufgabe
1. Ergänzen sie die folgende BIN-DEC-HEX-Zahlentabelle: (Was bedeutet MSB bzw. LSB?)

_Meine Lösung:_

| BIN(MSB) | BIN | BIN | BIN(LSB) | DEC | HEX |
|----------|-----|-----|----------|-----|-----|
| 0        | 0   | 0   | 0        | 0   | 0   |
| 0        | 0   | 0   | 1        | 1   | 1   |
| 0        | 0   | 1   | 0        | 2   | 2   |
| 0        | 0   | 1   | 1        | 3   | 3   |
| 0        | 1   | 0   | 0        | 4   | 4   |
| 0        | 1   | 0   | 1        | 5   | 5   |
| 0        | 1   | 1   | 0        | 6   | 6   |
| 0        | 1   | 1   | 1        | 7   | 7   |
| 1        | 0   | 0   | 0        | 8   | 8   |
| 1        | 0   | 0   | 1        | 9   | 9   |
| 1        | 0   | 1   | 0        | 10  | A   |
| 1        | 0   | 1   | 1        | 11  | B   |
| 1        | 1   | 0   | 0        | 12  | C   |
| 1        | 1   | 0   | 1        | 13  | D   |
| 1        | 1   | 1   | 0        | 14  | E   |
| 1        | 1   | 1   | 1        | 15  | F   |

MSB steht für "Most Significant Bit" (höchstwertiges Bit), und LSB steht für "Least Significant Bit" (niederwertigstes Bit). In einem Binärzahlensystem repräsentiert das MSB das Bit mit dem höchsten Wert (2*(n-1)), während das LSB das Bit mit dem niedrigsten Wert (2*0) ist.

2. Wandeln sie die folgende Dezimalzahl ohne Taschenrechner in die entsprechende Binärzahl um: 911

_Meine Lösung:_

911 ÷ 2 = 455 Rest 1
455 ÷ 2 = 227 Rest 1
227 ÷ 2 = 113 Rest 1
113 ÷ 2 = 56  Rest 0
56  ÷ 2 = 28  Rest 0
28  ÷ 2 = 14  Rest 0
14  ÷ 2 = 7   Rest 0
7   ÷ 2 = 3   Rest 1
3   ÷ 2 = 1   Rest 1
1   ÷ 2 = 0   Rest 1
Die Binärzahl von 911 ist 1110001111.

3. Wandeln sie die folgende Binärzahl ohne Taschenrechner in die entsprechende Dezimalzahl um: 1011'0110

_Meine Lösung:_

1 × 2^7 + 0 × 2^6 + 1 × 2^5 + 1 × 2^4 + 0 × 2^3 + 1 × 2^2 + 1 × 2^1 + 0 × 2^0

= 128 + 0 + 32 + 16 + 0 + 4 + 2 + 0

= 182

4. Wandeln sie die folgende Binärzahl ohne Taschenrechner in die entsprechende Hexadezimalzahl um: 1110'0010'1010'0101

_Meine Lösung:_

1110 0010 1010 0101

1110 -> E (entspricht der Dezimalzahl 14)
0010 -> 2 (entspricht der Dezimalzahl 2)
1010 -> A (entspricht der Dezimalzahl 10)
0101 -> 5 (entspricht der Dezimalzahl 5)

Die Hexadezimalzahl ist E2A5.



-----------
### 1.3 Reflexion 
Wir haben mit dem Thema "Daten codieren" begonnen. Unser Lehrer hat uns eine interessante Anekdote über ein Schachspiel erzählt, die uns verdeutlicht hat, wie wichtig das Codieren von Daten sein kann. Wir haben das Dokument "Schachbrett.pdf" erhalten, um die Anekdote besser zu verstehen. Anschließend wurden wir aufgefordert, eine kurze Übung mit einer Java-IDE durchzuführen. Wir sollten die Anzahl der Reiskörner auf dem letzten Schachfeld berechnen. Dabei haben wir verschiedene Konzepte wie Datentypen, Wertebereich, Ganzzahlen (mit oder ohne Vorzeichen) und Fliesskommazahlen diskutiert. Besonders interessant fand ich die Diskussion über die Formatierung und Genauigkeit von Fliesskommazahlen. Wir haben gelernt, wie wir eine Datei mit einem HEX-Editor analysieren können, zum Beispiel mit dem Online-Editor "hexed.it". Dabei haben wir auch über verschiedene Zahlensysteme wie Dual/Binär, Oktal und HEX sowie numerische Codes gesprochen. In den letzten zwei Stunden haben wir Zeit bekommen verschiedene Aufgaben zu lösen zum Thema Zahlensysteme. 

### Tag 2 [23.05.2023]

-----------
### 2.1 Theorie 
#### 2er Komplement 
Der 2er-Komplement-Code ist eine Methode zur Darstellung von negativen Zahlen in Computern. Im 2er-Komplement wird die negative Darstellung einer Zahl durch die Invertierung aller Bits (Nullen werden zu Einsen und Einsen werden zu Nullen) und die Addition von Eins zum Ergebnis der Invertierung erreicht.
#### ASCII: (American Standard Code for Information Interchange)
ASCII ist ein Zeichensatz, der in Computern weit verbreitet ist und zur Darstellung von Text verwendet wird. Es ist ein 7-Bit-Code, der 128 verschiedene Zeichen enthält, darunter Buchstaben, Zahlen, Satzzeichen und Steuerzeichen. Jedes Zeichen wird durch eine spezifische binäre Zahl repräsentiert. Zum Beispiel wird der Buchstabe "A" durch die Zahl 65 dargestellt. ASCII war einer der ersten standardisierten Zeichensätze und ist nach wie vor weit verbreitet, insbesondere in englischsprachigen Ländern.
#### Unicode
Unicode ist ein internationaler Zeichensatz, der entwickelt wurde, um eine umfassende Darstellung von Schriftzeichen aller Schriftsysteme der Welt zu ermöglichen. Im Gegensatz zu ASCII ist Unicode ein 16-Bit- oder 32-Bit-Code und kann somit eine viel größere Anzahl von Zeichen darstellen. Unicode umfasst Zeichen aus verschiedenen Sprachen, Symbole, Emojis und Sonderzeichen. Es ermöglicht eine standardisierte Darstellung von Texten in verschiedenen Sprachen und ist in der heutigen globalisierten Welt von großer Bedeutung.

-----------
### 2.2 Aufgaben
Zahlensystem

5. Der Addierer einer ALU erhält für Zahl-A: 1101'1001 und für Zahl-B: 0111'0101. Was wird man als Resultat erhalten? Erklären sie!

_Meine Lösung:_

Das Ergebnis der Addition von Zahl A (1101 1001) und ZahlB (0111 0101) ist  0100 1110.

6. Sie analysieren mit den Network-Sniffer Wireshark ihren Network-Traffic. Sie haben in OSI-Layer3 unter anderem folgende Bitkombination herausgelesen:
1100 0000 . 1010 1000 . 0100 1100 . 1101 0011
Was bedeuet dies? Beantworten sie diese Frage möglichst umfassend.
(BTW: Wer für diese und alle weiteren Umrechnungen den Taschenrechner benutzt, betrügt sich selbst ;-)

_Meine Lösung:_
Die Bitkombination, lässt sich in vier Oktette aufteilen: 1100 0000, 1010 1000, 0100 1100 und 1101 0011. Aus diese Okete kann man ein IPv4 Adresse bilden. Das erste Oktett 1100 0000 entspricht in dezimaler Form der Zahl 192.
Das zweite Oktett 1010 1000 entspricht in dezimaler Form der Zahl 168.
Das dritte Oktett 0100 1100 entspricht in dezimaler Form der Zahl 76.
Das vierte Oktett 1101 0011 entspricht in dezimaler Form der Zahl 211.

Zusammenergibt sich die IP-Adresse: 192.168.76.211.

8. In einer LINUX-Shell (Terminal) entdecken sie folgende Programmzeile:
chmod 751 CreateWeeklyReport
Was bedeuet dies? Beantworten sie diese Frage möglichst umfassend.

_Meine Lösung:_

Der Befehl "chmod" steht für "change mode" und ermöglicht die Veränderung der Zugriffsrechte von Dateien und Verzeichnissen in Linux.

Die erste Ziffer (7) repräsentiert die Zugriffsrechte für den Eigentümer der Datei. In diesem Fall erhält der Eigentümer volle Rechte (Lesen, Schreiben und Ausführen).

Die zweite Ziffer (5) repräsentiert die Zugriffsrechte für die Gruppe, der die Datei gehört. In diesem Fall erhält die Gruppe Leserechte und Ausführungsrechte, jedoch keine Schreibrechte.

Die dritte Ziffer (1) repräsentiert die Zugriffsrechte für andere Benutzer, die nicht Eigentümer sind und nicht zur Gruppe gehören. In diesem Fall haben andere Benutzer nur Ausführungsrechte, jedoch keine Leserechte oder Schreibrechte.

Die Zahl "751" bedeutet, dass der Eigentümer volle Rechte hat, die Gruppe Lese- und Ausführungsrechte hat und andere Benutzer nur Ausführungsrechte haben.

ASCII & UNICODE
1. Welche der Dateien ist nun ASCII-codiert, welche UTF-8 und welche UTF-16 BE-BOM?

_Meine Lösung:_
Wenn man die Dateien auf Notepad++ öffnet und auf die Option Coding klickt sieht man welche Zeichencodierung für die Dateien verwendet wird.
Testsample1=ASCII, Testsample2=UTF-8, Testsample3=UTF-16 BE-BOM

2. Alle drei Dateien enthalten denselben Text. Aus wie vielen Zeichen besteht dieser?

_Meine Lösung:_
Der Text besteht aus 64 Zeichen. 

5. Big-Endian (BE): Bei Big-Endian werden die Bytes eines Zeichens in aufsteigender Reihenfolge von links nach rechts angeordnet. Das bedeutet, dass das höchstwertige Byte (Most Significant Byte, MSB) zuerst steht und das niederwertigste Byte (Least Significant Byte, LSB) zuletzt kommt. Diese Reihenfolge entspricht der natürlichen Schreibweise von Zahlen in menschenlesbarer Form. 
  
_Meine Lösung:_
- Big-Endian (BE): Bei Big-Endian werden die Bytes eines Zeichens in aufsteigender Reihenfolge von links nach rechts angeordnet. Das bedeutet, dass das höchstwertige Byte (Most Significant Byte, MSB) zuerst steht und das niederwertigste Byte (Least Significant Byte, LSB) zuletzt kommt. Diese Reihenfolge entspricht der natürlichen Schreibweise von Zahlen in menschenlesbarer Form. 

- Little-Endian (LE): Im Gegensatz dazu werden bei Little-Endian die Bytes eines Zeichens in umgekehrter Reihenfolge angeordnet, also vom LSB zum MSB. Das niedrigstwertige Byte steht zuerst und das höchstwertige Byte steht zuletzt. 


-----------
### 2.3 Reflexion 
Heute haben wir Zeit bekommen weiter an den Aufgaben zu arbeiten bezüglich der Zahlensysteme. Danach haben wir uns mit einem neuen Thema auseinander gesetzt. Die Beschäftigung mit den verschiedenen alphanumerischen Codes wie dem 7-Bit-ASCII-Code, dem 8-Bit-ASCII-Code, und den verschiedenen Varianten des Unicode (UTF-8, UTF-16 und UTF-32) hat mir einen tieferen Einblick in die komplexe Welt der Zeichenkodierung und Textdarstellung in der Computertechnologie gegeben. Wir haben auch Aufgaben über dieses Thema bekommen. 

### Tag 3 [30.05.2023]
### 3.1 Theorie 
Das additive Farbmodell (RGB) basiert auf der Idee, dass durch das Hinzufügen von Licht in den Grundfarben Rot, Grün und Blau verschiedene Farben erzeugt werden können. Indem diese drei Farben in unterschiedlichen Intensitäten miteinander kombiniert werden, entstehen die verschiedenen Farbtöne. Bei maximaler Intensität aller drei Farben erscheint Weiß, während bei keiner Intensität Schwarz entsteht. Das RGB-Farbmodell wird in digitalen Displays, Monitoren, Fernsehern und anderen Lichtquellen verwendet.

Das subtraktive Farbmodell (CMYK) hingegen basiert auf der Idee, dass Farben durch die Absorption oder Subtraktion von Licht erzeugt werden. Die Grundfarben Cyan, Magenta, Gelb und Schwarz (Key) werden auf weißem Papier oder einem anderen hellen Hintergrund gedruckt und absorbieren Licht in unterschiedlichem Maße. Durch die Kombination dieser Farben in verschiedenen Intensitäten entstehen andere Farben. Das CMYK-Farbmodell wird in der Druckindustrie verwendet, da es besser die Eigenschaften von Farbstoffen und Tinten repräsentiert.

Der Hauptunterschied zwischen RGB und CMYK liegt in ihrer Anwendung und den Farbabweichungen, die auftreten können. RGB eignet sich besser für die Darstellung von Farben in digitalen Anwendungen, da es die Eigenschaften von Lichtquellen widerspiegelt. CMYK hingegen ist besser geeignet für den Druck, da es die Eigenschaften von Farbstoffen und Tinten besser darstellt.
### 3.2 Aufgaben
FF0000 entspricht der Farbe .... -> rot
00FF00 entspricht der Farbe .... -> grün
0000FF entspricht der Farbe .... -> blau
FFFF00 entspricht der Farbe .... -> gelb
00FFFF entspricht der Farbe .... -> cyan
FF00FF entspricht der Farbe .... -> magenta
000000 entspricht der Farbe .... -> schwarz
FFFFFF entspricht der Farbe .... -> weiss
00BC00 entspricht der Farbe ... -> dunkel/militär grün

(nochmal anschauen)
C:0%, M:100%, Y:100%, K:0% entspricht der Farbe Cyan
C:100%, M:0%, Y:100%, K:0% entspricht der Farbe Magenta
C:100%, M:100%, Y:0%, K:0% entspricht der Farbe Gelb
C:0%, M:0%, Y:100%, K:0% entspricht der Farbe Blau
C:100%, M:0%, Y:0%, K:0% entspricht der Farbe Rot
C:0%, M:100%, Y:0%, K:0% entspricht der Farbe Grün
C:100%, M:100%, Y:100%, K:0% entspricht der Farbe Weiss
C:0%, M:0%, Y:0%, K:100% entspricht der Farbe Schwarz
C:0%, M:0%, Y:0%, K:0% entspricht der Farbe Transparent
C:0%, M:46%, Y:38%, K:22% entspricht der Farbe Braun

RGB 255/255/255 ergibt in YCbCr:
Y: 1, Cb: 0, Cr: 0

RGB 0/0/0 ergibt in YCbCr:
Y: 0, Cb: 0, Cr: 0

Y: 1, Cb: 0, Cr: 0 entspricht der Farbe:
Diese Kombination repräsentiert eine helle Farbe, wobei die Cb- und Cr-Komponenten neutral sind.

Y: 0, Cb: 0, Cr: 0 entspricht der Farbe:
Diese Kombination repräsentiert die Farbe Schwarz, da alle Komponenten auf Null gesetzt sind.

Y: 0, Cb: 1, Cr: 0 entspricht der Farbe:
Diese Kombination repräsentiert eine Farbe, bei der die Cb-Komponente den Blauanteil hervorhebt.

Y: 0, Cb: -1, Cr: 0 entspricht der Farbe:
Diese Kombination repräsentiert eine Farbe, bei der die Cb-Komponente den Gelbanteil verstärkt.

Y: 0, Cb: 0, Cr: 1 entspricht der Farbe:
Diese Kombination repräsentiert eine Farbe, bei der die Cr-Komponente den Rotanteil verstärkt.

Y: 0, Cb: 0, Cr: -1 entspricht der Farbe:
Diese Kombination repräsentiert eine Farbe, bei der die Cr-Komponente den Grünanteil verstärkt.

Y: 0.3, Cb: 0.5, Cr: -0.17 entspricht der Farbe:


1. Suchen sie im Internet ein Bild vom Matterhorn, das eine Grösse von mind. 3000 Pixel aufweist und laden sie es auf ihren Notebook herunter. Danach bearbeiten sie es in einer Bildbearbeitungs-Software ihrer Wahl. Empfohlen wird das Online-Bildbearbeitungswerkzeug auf www.pixlr.com.
Da das Bild eine viel zu hohe Auslösung hat, rechnen sie es herunter. Bei dieser Gelegenheit ändern sie das Bildseitenverhältnis auf 16:9. Sie werden sich für einen Bldauschschnitt entscheiden müssen. Das Bild soll schlussendlich 720 Bildzeilen ausweisen.
Speichern sie das Bild als JPG in höchster und tiefster Qualität ab, zudem auch als PNG ohne Transparenz. Notieren sie sich die erfoderlichen Speichergrössen. Im Anschluss berechnen sie den unkomprimierten, theoretischen Speicherbedarf bei 8 Bit pro Farbkanal in MiB. Vergleichen sie die Werte und erklären sie die Unterschiede.

_Meine Lösung:_
PNG ist ein verlustfreies Format, das eine höhere Dateigröße im Vergleich zu JPG aufweisen kann, da es keine Datenkompression mit Qualitätsverlust verwendet. Die höchste Qualitätseinstellung beim Speichern als JPG führt zu einer größeren Dateigröße, da das Bild weniger komprimiert wird und somit mehr Details beibehält. Die niedrigste Qualitätseinstellung beim Speichern als JPG führt zu einer geringeren Dateigröße, da das Bild stärker komprimiert wird und somit mehr Informationen verloren gehen, was zu einer geringeren visuellen Qualität führen kann.

Bei PNG-Dateien ohne Transparenz wird eine verlustfreie Kompression verwendet, die die Dateigröße reduziert, aber im Allgemeinen eine größere Dateigröße als JPG ergibt. Die Unterschiede in den Speichergrößen zwischen den verschiedenen Formaten und Qualitätsstufen zeigen die Kompromisse zwischen Dateigröße und visueller Qualität. Höhere Qualitätsstufen und verlustfreie Formate wie PNG erzeugen größere Dateien, behalten jedoch mehr Details und visuelle Qualität bei. Niedrigere Qualitätsstufen und verlustbehaftete Formate wie JPG erzeugen kleinere Dateien, weisen jedoch einen geringeren Detailgrad und eine geringere visuelle Qualität auf.

2. Berechnen sie den Speicherbedarf für ein unkomprimiertes Einzelbild im HD720p50-Format bei einer True-Color-Farbauflösung. (Die Begriffe HD720p50 und TrueColor bitte googeln)


_Meine Lösung:_
Das HD720p50-Format bezieht sich auf eine HD-Auflösung mit einer Bildwiederholfrequenz von 50 Bildern pro Sekunde. Es hat eine Bildgröße von 1280 x 720 Pixeln (Breite x Höhe).

True-Color-Farbauflösung bedeutet, dass für jeden der drei Farbkanäle (Rot, Grün, Blau) 8 Bit verwendet werden, was insgesamt 24 Bit pro Pixel ergibt.

Um den Speicherbedarf für ein unkomprimiertes Einzelbild im HD720p50-Format zu berechnen, verwenden wir folgende Schritte:

Multiplizieren Sie die Breite und Höhe des Bildes, um die Gesamtzahl der Pixel zu erhalten: 1280 x 720 = 921.600 Pixel.

Multiplizieren Sie die Anzahl der Pixel mit 24 (8 Bit pro Farbkanal x 3 Kanäle) und teilen Sie das Ergebnis durch 8, um die Anzahl der Bytes zu erhalten: (921.600 x 24) / 8 = 2.764.800 Bytes.

Um den Speicherbedarf in MiB zu berechnen, teilen Sie die Anzahl der Bytes durch 1024^2 (1024 hoch 2): 2.764.800 Bytes / 1024^2 ≈ 2,64 MiB.

Daher beträgt der unkomprimierte Speicherbedarf für ein Einzelbild im HD720p50-Format mit True-Color-Farbauflösung etwa 2,64 MiB.

3. Ihre Digitalkamera bietet für die Speicherung ihrer Bilder folgende Formate an: RAW, TIF, JPG. Erklären sie in ein paar kurzen Sätzen die Unterschiede und Einsatzgebiete dieser drei Formatvarianten.

_Meine Lösung:_
RAW: Das RAW-Format ist ein unkomprimiertes und verlustfreies Dateiformat, das die rohen Bilddaten direkt von der Kamera speichert. Es enthält alle Informationen, die von den Bildsensoren erfasst wurden, ohne jegliche Verarbeitung oder Kompression. RAW-Dateien bieten maximale Flexibilität bei der Bildbearbeitung, da sie es ermöglichen, Belichtung, Weißabgleich, Kontrast und andere Parameter nachträglich anzupassen. Es wird oft von professionellen Fotografen und fortgeschrittenen Nutzern bevorzugt, die eine umfassende Kontrolle über den Bearbeitungsprozess wünschen.

TIF (Tagged Image File Format): TIF ist ein verlustfreies Dateiformat, das eine hohe Bildqualität beibehält. Es unterstützt verschiedene Farbmodelle und Tiefen, einschließlich 8-Bit- und 16-Bit-Pro-Channel-Farbunterstützung. TIF-Dateien werden häufig für die Archivierung und den Austausch von Bildern verwendet. Sie eignen sich gut für die professionelle Druckvorstufe, die Grafikbearbeitung und die langfristige Aufbewahrung von Bildern.

JPG (Joint Photographic Experts Group): JPG ist ein komprimiertes Dateiformat, das eine effiziente Speicherung von Bildern ermöglicht. Es verwendet eine verlustbehaftete Kompression, bei der Daten entfernt werden, um die Dateigröße zu reduzieren. Dies kann zu einem Qualitätsverlust führen, insbesondere bei starken Komprimierungseinstellungen. JPG-Dateien sind platzsparend und weit verbreitet, sodass sie sich gut für den Online-Austausch von Bildern und die Anzeige auf Bildschirmen eignen. Sie eignen sich jedoch weniger für umfangreiche Bearbeitungen, da bei jeder erneuten Speicherung Kompressionsartefakte auftreten können.


### 3.3 Reflexion 
 Die Einführung in die Bildcodierung hat mir gezeigt, wie vielfältig und nützlich Barcodes und QR-Codes sein können. Der Unterschied zwischen Bitmap/Rastergrafik und Vektorgrafik wurde deutlich, indem ich erkannte, dass Bitmaps aus einzelnen Pixeln bestehen und für detaillierte Bilddarstellungen geeignet sind, während Vektorgrafiken auf mathematischen Formeln basieren und sich besser für skalierbare Bilder eignen. Die Unterscheidung zwischen DPI (Dots Per Inch) und PPI (Pixels Per Inch) war wichtig, um die Auflösung und Qualität von Bildern besser zu verstehen. DPI bezieht sich auf die Druckqualität, während PPI die Bildschirmauflösung beschreibt. Abschließend haben wir eine kurze Einführung in die Analog-Digital-Wandlung erhalten, die mir einen Einblick in den Prozess der Umwandlung von analogen Signalen in digitale Daten gegeben hat.

### Tag 4 [6.6.2023]
### 4.1 Theorie 
Ein Codec steht für "Codierer/Dekodierer" und bezieht sich auf einen Algorithmus oder eine Software, die für die Kompression und Dekompression von Medieninhalten verwendet wird. Ein Codec kann verschiedene Arten von Daten komprimieren, wie Audio, Video oder Bilder. Während der Kompression werden redundante oder unwichtige Informationen entfernt, um die Dateigröße zu verringern, während bei der Dekompression die Daten wiederhergestellt werden. Bekannte Beispiele für Codecs sind H.264, MPEG-4 und AAC.
Beispiele zu Video-Codecs:
♦ Cinepak ♦ Sorenson ♦ Sorenson3 ♦ DV-PAL ♦ DV-NTSC ♦ MPEG-1 ♦ MPEG-2 ♦ MPEG-4 ♦ MPEG-4 Implementierungen DivX, Xvid und AVCHD ♦ H.261 ♦ H.263 ♦ H.264 ♦ H.265 ♦ Flashvideo FLV und F4V ♦ Theora ♦ RealVideo ♦ 3rd Generation Partnership Project für Smartphone 3GPP ♦ Windows Media Video wmv
Beispiele zu Audio-Codecs:
♦ MPEG1 Layer 2 ♦ MPEG1 Layer3 → MP3 ♦ Ogg Vorbis ♦ RealAudio ♦ Windows Media Audio wma

Ein Container hingegen ist ein Dateiformat, das verschiedene Arten von Medieninhalten zusammenfasst und speichert. Ein Container kann sowohl komprimierte als auch unkomprimierte Daten enthalten und bietet zusätzliche Funktionen wie Metadaten (Informationen über das Medium) und Synchronisation von Audio und Video. Containerformate sind üblicherweise für die Wiedergabe und das Streaming von Medieninhalten auf verschiedenen Geräten geeignet. 
Beispiele zu Audio/Video-Containers:
Microsoft AVI → Audio-Video Interleave ♦ ADOBE Flash Video ♦ Apple Quicktime mov ♦ Blu-ray Disc ♦ DVD ♦ MPEG-2 Stream ♦ RealMedia

Quelle: https://www.juergarnold.ch/videotechnik.html#mm_4_6

### 4.2 Aufgaben
Qualitätsvergleiche von Frequenzen und Auflösungen: https://www.juergarnold.ch/videotechnik.html#mm_6_3


4. Sie möchten ihr neulich erstelltes Gameplay-Video auf Youtube veröffentlichen. Was sind die technischen Vorgaben dazu? (Format, Bildrate, Farbauflösung, Video-, Audiocodec etc.). Gibt es allenfalls rechtliche Einschränkungen?

_Meine Lösung:_
Videoformat: YouTube unterstützt verschiedene Videoformate wie MP4, MOV, AVI, WMV und mehr. Das empfohlene Format ist jedoch MP4, da es eine gute Kompatibilität und Qualität bietet.

Bildrate: YouTube akzeptiert eine Vielzahl von Bildraten, darunter 24, 25, 30, 48, 50, 60, 120 und 240 Bilder pro Sekunde. Die Wahl der Bildrate hängt von Ihrem Gameplay und den Aufnahmeeinstellungen ab. Eine gängige Bildrate ist 30 FPS (Frames per Second).

Auflösung: YouTube unterstützt eine breite Palette von Auflösungen. Es wird empfohlen, die höchstmögliche Auflösung zu verwenden, die für Ihr Gameplay und Ihre Aufnahmeeinstellungen geeignet ist. Gängige Auflösungen sind beispielsweise 720p (1280x720 Pixel), 1080p (1920x1080 Pixel) oder sogar 4K (3840x2160 Pixel).

Video- und Audiocodec: YouTube empfiehlt die Verwendung des H.264-Videoformats für die Komprimierung von Videos. Für den Audiocodec wird AAC mit einer Bitrate von mindestens 128 kbps empfohlen.

Dateigröße: YouTube hat eine Begrenzung für die Dateigröße von hochgeladenen Videos. Die maximale Dateigröße beträgt normalerweise 128 GB oder 12 Stunden, je nachdem, welcher Wert zuerst erreicht wird.
### 4.3 Reflexion
Die Einführung in das Thema Komprimierung hat mir einen Einblick in die verschiedenen Arten der Datenkompression gegeben. Ich lernte den Unterschied zwischen verlustloser und verlustbehafteter Komprimierung kennen und erkannte die Vor- und Nachteile jeder Methode.  Die Auseinandersetzung mit dem Huffman-Algorithmus half mir dabei, die Grundlagen der verlustlosen Datenkompression besser zu verstehen. Ich erkannte, wie der Algorithmus die Häufigkeit von Zeichen in einer Nachricht analysiert und effiziente Codewörter zuweist, um die Datenmenge zu reduzieren. Ebenfalls haben wir die erste Prüfung geschrieben im Modul. 

### Tag 5 [13.06.2023]
### 5.1 Theorie 
RLC (Run Length Coding) bzw. RLE (Run Length Encoding) ist ein einfaches verlustloses Komprimierungsverfahren, das auf der Wiederholung von aufeinanderfolgenden Daten basiert. Es erkennt Sequenzen von gleichen Zeichen oder Symbolen und codiert sie als eine einzelne Instanz des Zeichens zusammen mit der Anzahl der Wiederholungen. Dadurch wird die Datenmenge reduziert, insbesondere bei wiederholenden Mustern.

Das lexikalische Verfahren LZW (Lempel-Ziv-Welch-Algorithmus) ist ein verlustfreier Komprimierungsalgorithmus, der auf einer Wörterbuchtechnik basiert. Es erkennt und codiert wiederholende Zeichenketten oder Muster, indem es sie durch eine kürzere Codewortrepräsentation ersetzt. Das Wörterbuch wird während der Codierung dynamisch erweitert, um neue Zeichenketten zu erfassen. Dieser Algorithmus eignet sich gut für Textdaten und hat eine hohe Kompressionsrate.

Der Huffman-Algorithmus ist ein verlustfreier Kompressionsalgorithmus, der auf einer statistischen Analyse der Häufigkeit von Zeichen basiert. Er ordnet häufig verwendeten Zeichen kürzere Codewörter und weniger verwendeten Zeichen längere Codewörter zu, um eine effiziente Codierung zu erreichen. Der Huffman-Algorithmus verwendet eine Baumstruktur, in der die Codewörter durch den Pfad vom Wurzelknoten zu den Blattknoten abgeleitet werden. Dieser Algorithmus wird häufig für die Komprimierung von Text-, Bild- und Tondaten verwendet.

Jeder Algorithmus hat seine eigenen Stärken und Schwächen und kann je nach Art der Daten und Kompressionsanforderungen eingesetzt werden.
### 5.2 Aufgaben
1. Huffman-Algorithmus: (Teamarbeit). Jeder denkt für sich ein Wort mit ca. 15 Buchstaben aus und erstellt dazu die Huffman-Codetabelle und das entsprechend komprimierte Wort in HEX-Darstellung. Nun werden die Codes inklusive der Codetabelle gegenseitig ausgetauscht. Kann ihr Partner ihr gewähltes Wort richtig dekomprimieren?

_Meine Lösung:_
Buchstaben und ihre Häufigkeiten: H (1), u (1), f (2), m (2), a (1), n (1).

Baum: 
       Root
       ├── f (2)
       │   ├── H (1)
       │   └── u (1)
       └── n (2)
           ├── m (1)
           └── a (1)

Codetabelle: 
H: 00
u: 01
f: 10
m: 110
a: 111
n: 111

Wort: "Huffman"
2. RLC/E-Verfahren: Sie erhalten diesen RL-Code:
010100011110010010010010010010010010010110010110010010010010010010010010001
Folgendes ist ihnen dazu bekannt: Es handelt sich um eine quadratische Schwarz-Weiss-Rastergrafik mit einer Kantenlänge von 8 Pixel. Es wird links oben mit der Farbe Weiss begonnen. Eine Farbe kann sich nicht mehr als siebenmal wiederholen. Zeichnen sie die Grafik auf. Was stellt sie dar?

_Meine Lösung:_
Es sollte einen Quadrat darstellen. 

3. LZW-Verfahren: Erstellen sie die LZW-Codierung für das Wort «ANANAS» und überprüfen sie mit der Dekodierung ihr Resultat. Danach versuchen sie den erhaltenen LZW-Code «ERDBE<256>KL<260>» zu dekomprimieren.  

_Meine Lösung:_
1. "A" zur aktuellen Sequenz hinzufügen.
2. Überprüfen, ob die Sequenz bereits im Wörterbuch vorhanden ist.
3. "N" zur aktuellen Sequenz hinzufügen und "AN" erhalten.
4. Überprüfen, ob die Sequenz "AN" bereits im Wörterbuch vorhanden ist.
5. Die Schritte 5-7 für die restlichen Zeichen "A", "N", "A" und "S" wiederholen.
Die LZW-Codierung für das Wort "ANANAS" lautet: 0 1 2 4 3.

### 5.3 Reflexion 
Zu Begin haben wir eine Prüfungsbesprechung gemacht zu der Prüfung, die wir ansolviert haben letzte Woche. Danach haben wir eine kurze Einführung in die Themen RLC,RLE und Verlustbehaftete Komprimierung bekommen. Die Einführung in die verlustbehaftete Komprimierung von Bild- und Tondaten eröffnete mir die Welt der Techniken, die bei der Reduzierung der Datenmenge unter Berücksichtigung der Wahrnehmung des menschlichen Sinnes angewendet werden. Es wurde deutlich, dass bei der verlustbehafteten Komprimierung eine Abwägung zwischen Qualität und Dateigröße erfolgen muss. Wir haben auch Zeit bekommen uns selbstständig in den verschiede Themenbereiche zu vertiefen. 

### Tag 6 [20.6.2023]
### 6.1 Theorie 
Klassische symmetrische Verfahren wie ROT, Vigenere und XOR sind Verschlüsselungsverfahren, die in der Kryptographie eingesetzt werden. ROT (Rotation) ist eine einfache Verschlüsselungsmethode, bei der jeder Buchstabe im Klartext um einen festgelegten Wert verschoben wird. Zum Beispiel wird bei ROT-13 jeder Buchstabe um 13 Positionen im Alphabet verschoben. ROT-Verschlüsselung ist ein symmetrisches Verfahren, da derselbe Schlüssel zum Verschlüsseln und Entschlüsseln verwendet wird. Es handelt sich jedoch um eine sehr schwache Verschlüsselungsmethode, da es nur 25 mögliche Verschiebewerte gibt.

Vigenere ist eine polyalphabetische Verschlüsselungsmethode, bei der eine Schlüsselwortphrase verwendet wird, um den Klartext zu verschlüsseln. Jeder Buchstabe des Schlüsselworts bestimmt die Verschiebung, die auf den entsprechenden Buchstaben im Klartext angewendet wird. Dies ermöglicht eine stärkere Verschlüsselung als ROT, da die Verschiebung für jeden Buchstaben im Klartext unterschiedlich sein kann.

XOR (Exklusives Oder) ist ein bitweises Verknüpfungsverfahren, das häufig in der symmetrischen Verschlüsselung verwendet wird. Beim XOR-Verschlüsseln werden die Bits des Klartexts mit den entsprechenden Bits eines Schlüssels kombiniert, um den Geheimtext zu erzeugen. Die Entschlüsselung erfolgt durch erneutes Anwenden des XOR-Verfahrens mit demselben Schlüssel. 


### 6.2 Aufgaben
1. Die Rotationschiffre:
Schon der römische Feldherr und spätere Kaiser Julius Cäsar kannte den folgenden Verschlüsselungstrick und nutzte ihn bei seinen geheimen Botschaften: Ersetze jeden Buchstaben durch den, der eine bestimmte Anzahl Stellen später im Alphabet folgt! Somit konnte Cäsar effektiv geheime Botschaften übermitteln, wie z.B. diese Zitate:
GHU DQJULII HUIROJW CXU WHHCHLW GLH ZXHUIHO VLQG JHIDOOHQ LFK NDP VDK XQG VLHJWH WHLOH XQG KHUUVFKH
Benutzen Sie nun Ihr CrypTool1 und finden Sie heraus, um welche Zitate es sich handelt! Die Rotationschiffre ist übrigens ein klassisches, symmetrisches Verfahren. Nun aber nicht einfach drauflos probieren. Machen Sie etwas Kryptoanalyse mit einem ASCII-Histogramm. (Tipp: Häufigkeitsanalyse der vorkommenden Buchstaben)

_Meine Lösung:_
DER ANGRIFF ERFOLGT ZUR TEEZEIT DIE WUERFEL SIND GEFALLEN ICH KAM SAH UND SIEGTE TEILE UND HERRSCHE

2. Vigenèreverschlüsselung: 
Um etwas warm zu laufen, verschlüsseln wird ohne Cryptool (!) das Wort BEEF mit dem Schlüsselwort AFFE.
Danach, wiederum ohne Cryptool, entschlüsseln wir den Geheimtext WRKXQT mit dem Schlüsselwort SECRET.
Nun wirds wirklich spannend: Wir versuchen den Vigenère-Code zu knacken und bedienen uns einem Analysewerkzeug im Cryptool1. Heimlich abgehört haben wir die folgende Vigenère-Chiffre:
USP JHYRH ZZB GTV CJ WQK OCLGQVFQK GAYKGVFGX NS ISBVB MYBC MWCC NS JOEVB GTV KRQFV AGK XCUSP VFLVBLLBE ESSEILUBCLBXZU SENSWFGVRCES SER CZBCE ILUOLBPYISL CCSZG VZJ
Neugierig wie wir sind, möchten wir gerne wissen, welcher Text hinter dieser Chiffre steckt. Da uns aber das Schlüsselwort fehlt, müssen wir tief in unsere Trickkiste greifen. (Tipp: Im CrypTool1/Hilfe/Index/Vigenère-Verschlüsselungsverfahren findet man weitere Informationen zum Vigenère-Analyseverfahren.)

_Meine Lösung:_
Key = ROY
DER STAAT BIN ICH ES IST AEUSSERST SCHWIERIG ZU REDEN OHNE VIEL ZU SAGEN ICH MACHE MIT JEDER ERNENNUNG NEUNUNDNEUNZIG UNZUFRIEDENE UND EINEN UNDANKBAREN LOUIS XIV
### 6.3 Reflexion 
Das Kahoot Spiel hat geholfen das gerlernte nochmals zu repetieren. Im Anschluss daran haben wir uns mit der Intraframe-Komprimierung beschäftigt. Dabei ging es um verschiedene Techniken wie die Reduzierung der Auflösung, die diskrete Kosinustransformation (DCT) und Subsampling, die innerhalb eines Bildes angewendet werden. Nachdem wir alle Aufgaben zu Kompression und Multimedia abgeschlossen hatten, haben wir uns einem neuen Thema zugewandt: Kryptologie, Kryptografie und Kryptoanalyse. Wir begannen mit dem Einsatz des Tools "Crypttool1", einem Labor für Kryptografie und Analyse. Dies ermöglichte uns, uns mit klassischen symmetrischen Verfahren wie ROT, Vigenere und XOR zu beschäftigen. Wir lernten verschiedene Verschlüsselungsmethoden kennen und wie sie angewendet werden.
### Tag 7 [27.06.2023]
### 7.1 Theorie
Hybride Verschlüsselungsverfahren kombinieren die Vorteile von asymmetrischen (öffentlichen) und symmetrischen (geheimen) Verschlüsselungsverfahren, um eine effiziente und sichere Kommunikation zu ermöglichen.

Der Ablauf eines hybriden Verschlüsselungsverfahrens sieht wie folgt aus:

1. Der Sender generiert zunächst einen zufälligen symmetrischen Sitzungsschlüssel, der für die Verschlüsselung der eigentlichen Daten verwendet wird. Dieser Sitzungsschlüssel ist geheim und wird nicht über das Netzwerk übertragen.

2. Der öffentliche Schlüssel des Empfängers wird verwendet, um den Sitzungsschlüssel asymmetrisch zu verschlüsseln. Nur der Empfänger kann den Sitzungsschlüssel mit seinem privaten Schlüssel entschlüsseln.

3. Der verschlüsselte Sitzungsschlüssel wird zusammen mit den verschlüsselten Daten an den Empfänger gesendet.

4. Der Empfänger verwendet seinen privaten Schlüssel, um den verschlüsselten Sitzungsschlüssel zu entschlüsseln und den symmetrischen Sitzungsschlüssel zu erhalten.

5. Der symmetrische Sitzungsschlüssel wird verwendet, um die eigentlichen Daten symmetrisch zu verschlüsseln. Dieser Vorgang ist effizienter als die asymmetrische Verschlüsselung.

6. Die verschlüsselten Daten werden an den Empfänger übertragen.

7. Der Empfänger verwendet den symmetrischen Sitzungsschlüssel, um die verschlüsselten Daten zu entschlüsseln und den Klartext zu erhalten.

Durch die Kombination von asymmetrischer und symmetrischer Verschlüsselung profitiert das hybride Verfahren von der hohen Sicherheit der asymmetrischen Verschlüsselung für den sicheren Austausch des symmetrischen Sitzungsschlüssels, während die effiziente symmetrische Verschlüsselung für die eigentliche Datenübertragung verwendet wird. Auf diese Weise werden die Vorteile beider Verfahren genutzt, um eine sichere und effiziente Kommunikation zu gewährleisten.


### 7.2 Aufgaben
1. Spielen sie in Cryptool1 einen Schlüsseltausch gemäss Diffie-Hellman durch. Experimentieren sie mit verschiedenen, auch eigenen Parametern. (Sie finden das Tool unter Einzelverfahren→Protokolle→Diffie-Hellman-Demo...)

_Meine Lösung:_
![alice](/aliceBob.png) 
2. RSA-Verschlüsselung:
Erzeugen sie zwei asymmetrische Schlüsselpaare: Eines für «Muster Felix» und eines für «Hasler Harry» (Sie finden das Tool unter Digitale Signaturen/PKI→PKI→Schlüssel erzeugen/importieren...)
Verschlüsseln Sie nun eine Nachricht für Muster Felix und versuchen sie danach, den Text als Hasler Harry, danach als Muster Felix zu entschlüsseln. Was stellen sie fest? (Sie finden die Tools unter Ver-/Entschlüsseln→Asymmetrisch→RSA-Ver/Entschlüsselung...)

_Meine Lösung:_
+ Decrypt: 
![decyrptMessage](/decryptMessage.png) 

+ Encrypt: 
![encrypt](/encrypt.png)

Digital Signieren
1. Führen Sie nun im Cryptool die Hash-Demo aus. Sie finden diese unter Einzelverfahren → Hashverfahren → Hash-Demo...

_Meine Lösung:_

![hashdemo](/hashdemo.png)
2. Erstellen sie ein kurzes Dokument und signieren sie dieses.
Siehe Digitale Signaturen/PKI → Dokument signieren nzw. Dokument überprüfen.
Nehmen sie am signierten Dokument eine kleine Änderung vor und überprüfen sie die Signatur erneut. Was stellen sie fest?

_Meine Lösung:_
![signieren](/signieren.png)

Nach Änderung der Nachricht: 
![signieren](/changemessage.png)



### 7.3 Reflexion
Die Tätigkeiten haben mir einen Einblick in verschiedene Verschlüsselungsverfahren gegeben. Symmetrische Verschlüsselung hat den Nachteil, dass die Anzahl der Schlüssel quadratisch mit der Anzahl der Kommunikationspartner wächst und der Schlüsseltausch eine Herausforderung darstellt. Asymmetrische Verschlüsselung löst dieses Problem durch den Einsatz eines Schlüsselpaars und ermöglicht einen sicheren Schlüsseltausch. Hybride Verfahren kombinieren die Vorteile beider Ansätze. Hash-Wertbildung und digitale Signatur dienen der Datenintegrität und Authentizität. Insgesamt haben die Tätigkeiten mein Verständnis für Verschlüsselungsverfahren vertieft.

### Tag 8 [04.07.2023]
### 8.1 Theorie
PKI (Public Key Infrastructure) ist eine Infrastruktur, die die Verwaltung und den Einsatz von asymmetrischen Verschlüsselungsverfahren erleichtert. Sie basiert auf der Verwendung von Zertifikaten, die digitale Identitäten und öffentliche Schlüssel einer Person oder einer Organisation authentifizieren.

Zertifikate werden verwendet, um die Echtheit von öffentlichen Schlüsseln zu überprüfen und die Vertrauenswürdigkeit von Kommunikationspartnern zu gewährleisten. Für E-Mail-Verschlüsselung wird das OpenPGP-Protokoll verwendet, das auf dem PGP (Pretty Good Privacy) basiert. OpenPGP ermöglicht die Verschlüsselung, Signierung und Verifizierung von E-Mails durch den Einsatz von asymmetrischer Verschlüsselung.

Für die sichere Übertragung von Daten über das Internet, insbesondere bei HTTPS-Verbindungen, werden ebenfalls Zertifikate verwendet. Hier kommt das X.509-Standardformat zum Einsatz. Dabei wird ein Zertifikat von einer vertrauenswürdigen Zertifizierungsstelle (Certificate Authority) ausgestellt, die die Identität des Inhabers überprüft. Das Zertifikat enthält den öffentlichen Schlüssel des Servers und wird verwendet, um die sichere Kommunikation zwischen dem Client und dem Server mittels asymmetrischer Verschlüsselung und dem TLS (Transport Layer Security)-Protokoll zu ermöglichen.

Insgesamt bieten PKI und Zertifikate eine grundlegende Infrastruktur für die sichere Kommunikation über E-Mails und das Internet. Sie gewährleisten die Vertraulichkeit, Integrität und Authentizität der übertragenen Daten.

### 8.2 Aufgaben
Lehrerdemo

### 8.3 Reflexion
Es wurde erläutert, wie Zertifikate zur Authentifizierung von Kommunikationspartnern verwendet werden und wie die Verschlüsselung und Signierung von E-Mails mit PGP und OpenPGP funktioniert.

Ein weiterer Teil der Prüfungsbesprechung befasste sich mit der sicheren Datenübertragung über HTTPS und dem TLS-Protokoll. Es wurde eine Lehrerdemo durchgeführt, bei der eine Anfrage an einen HTTPS-Webserver mit Wireshark analysiert wurde. Dadurch konnte ich einen Einblick in den Ablauf der sicheren Datenübertragung gewinnen und die Bedeutung von TLS-Zertifikaten besser verstehen.

Eine weitere Lehrerdemo konzentrierte sich auf die Verwendung von pgp4win und Kleopatra. Dabei wurde gezeigt, wie man Schlüssel importiert und verschiedene Kombinationen von Verschlüsselung, Entschlüsselung und Signierung von Nachrichten durchführt. Diese praktischen Übungen haben mir geholfen, das Konzept der asymmetrischen Verschlüsselung besser zu verstehen und die Anwendung von PGP in der Praxis zu erlernen.








