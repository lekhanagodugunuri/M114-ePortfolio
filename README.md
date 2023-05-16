# M114-ePortfolio

## Inhaltsverzeichnis

### Tag 1 [16.05.2023]
#### Theorie 
hex editor

Zehner
Binär/Dual
Oktal
Hexadezimal


#### Aufgaben 
Theorie
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

Meine Lösung: 

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

Meine Lösung: 

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

Meine Lösung: 

1 × 2^7 + 0 × 2^6 + 1 × 2^5 + 1 × 2^4 + 0 × 2^3 + 1 × 2^2 + 1 × 2^1 + 0 × 2^0

= 128 + 0 + 32 + 16 + 0 + 4 + 2 + 0

= 182

4. Wandeln sie die folgende Binärzahl ohne Taschenrechner in die entsprechende Hexadezimalzahl um: 1110'0010'1010'0101

Meine Lösung:

1110 0010 1010 0101

1110 -> E (entspricht der Dezimalzahl 14)
0010 -> 2 (entspricht der Dezimalzahl 2)
1010 -> A (entspricht der Dezimalzahl 10)
0101 -> 5 (entspricht der Dezimalzahl 5)

Die Hexadezimalzahl ist E2A5.

5. Der Addierer einer ALU erhält für Zahl-A: 1101'1001 und für Zahl-B: 0111'0101. Was wird man als Resultat erhalten? Erklären sie!

  |   1101'1001  |
  |+ 0111'0101 |
  |__________|
  | 10100'1110  |


#### Reflexion 
Der Einstieg hat mit ziemlich viel Input angefangen. Wir haben einige Administrative Inputs bekommen und dann haben wir 2 Lektionen Inputs bekommen zu verschiedene Themen. 2 Lektionen haben wir jedoch auch Zeit bekommen uns mit Aufgaben zu beschäftigen. 