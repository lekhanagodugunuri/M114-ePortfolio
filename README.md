# M114-ePortfolio

## Inhaltsverzeichnis
- [Tag 1, 16.05.2023](#tag-1-16052023)
### Tag 1 [16.05.2023]
-----------
### Theorie 

#### Zahlensysteme 

Zahlensysteme und numerische Codes sind grundlegende Konzepte der Mathematik und Informatik, die verwendet werden, um Zahlen darzustellen, zu speichern und zu verarbeiten. In dieser Zusammenfassung werde ich auf Zahlensysteme, insbesondere das Dezimalsystem und das Binärsystem, sowie auf numerische Codes wie den Unsigned-Code und den Signed-Code eingehen.
Numerische Codes dienen dazu, Zahlen in einem bestimmten Format darzustellen. Der Unsigned-Code wird verwendet, um positive Zahlen darzustellen. Er verwendet alle verfügbaren Bits zur Darstellung des Zahlenwerts. Beispielsweise kann ein 8-Bit-Unsigned-Code Werte von 0 bis 255 darstellen. Der Signed-Code hingegen ermöglicht die Darstellung von sowohl positiven als auch negativen Zahlen. Er verwendet das erste Bit, das als Vorzeichenbit bezeichnet wird, um das Vorzeichen der Zahl anzugeben. 

#### Hex Editor  

Ein Hex-Editor ist ein spezielles Programm, das verwendet wird, um den Inhalt und die Struktur von Dateien auf binärer Ebene zu analysieren und zu bearbeiten. Hex-Editoren zeigen den Inhalt einer Datei in hexadezimaler Form an, wobei jedem Byte ein zweistelliger Hexadezimalwert zugeordnet wird. 
Vorteile: 
1. Analyse von Dateiformaten: Hex-Editoren ermöglichen es Entwicklern und Analysten, die Struktur und das Format von Dateien zu untersuchen. Da Dateien auf binärer Ebene gespeichert sind, ist es oft schwierig, den Inhalt mit einem Texteditor oder einem herkömmlichen Programm zu interpretieren. 
2. Datenbearbeitung: Hex-Editoren bieten die Möglichkeit, den Inhalt von Dateien direkt zu bearbeiten. Dies ist besonders hilfreich, wenn es erforderlich ist, bestimmte Werte oder Muster innerhalb einer Datei zu ändern. 
3. Datenrettung und Wiederherstellung: Bei der Datenrettung von beschädigten oder gelöschten Dateien können Hex-Editoren äußerst nützlich sein. Durch die direkte Analyse des binären Inhalts einer Datei ist es möglich, beschädigte oder fehlende Daten wiederherzustellen.
-----------
### Aufgaben 
#### Theorie
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
### Reflexion 
Wir haben mit dem Thema "Daten codieren" begonnen. Unser Lehrer hat uns eine interessante Anekdote über ein Schachspiel erzählt, die uns verdeutlicht hat, wie wichtig das Codieren von Daten sein kann. Wir haben das Dokument "Schachbrett.pdf" erhalten, um die Anekdote besser zu verstehen. Anschließend wurden wir aufgefordert, eine kurze Übung mit einer Java-IDE durchzuführen. Wir sollten die Anzahl der Reiskörner auf dem letzten Schachfeld berechnen. Dabei haben wir verschiedene Konzepte wie Datentypen, Wertebereich, Ganzzahlen (mit oder ohne Vorzeichen) und Fliesskommazahlen diskutiert. Besonders interessant fand ich die Diskussion über die Formatierung und Genauigkeit von Fliesskommazahlen. Wir haben gelernt, wie wir eine Datei mit einem HEX-Editor analysieren können, zum Beispiel mit dem Online-Editor "hexed.it". Dabei haben wir auch über verschiedene Zahlensysteme wie Dual/Binär, Oktal und HEX sowie numerische Codes gesprochen. In den letzten zwei Stunden haben wir Zeit bekommen verschiedene Aufgaben zu lösen zum Thema Zahlensysteme. 

