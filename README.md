# M114-ePortfolio

## Inhaltsverzeichnis
- [Tag 1, 16.05.2023](#tag-1-16052023)
- [Tag 2, 23.05.2023](#tag-2-23052023)
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
