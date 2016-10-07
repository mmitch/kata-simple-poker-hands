# Simple Poker Hands Kata

Diese Kata basiert auf der
[Poker Hands Kata](http://codingdojo.org/cgi-bin/index.pl?KataPokerHands),
ist aber stark vereinfacht.  Ich bin dieser Version der Kata schon
mehrfach begegnet, konnte sie aber nirgendwo im Internet finden und
verlinken, daher habe ich sie jetzt selbst mal aufgeschrieben.

## Ziel der Kata

Finde die beste Kombination (höchste einzelne Karte oder Paar)
innerhalb von 5 Karten.

## Karten

Eine Karte ist ein einfacher String, z.B. ``H10`` für die Herz-Zehn
oder ``PA`` für das Pik-Ass.

Ein Kartensatz besteht aus mehreren Karten, die durch Leerzeichen
getrennt sind:  ``K5 P1 H5 KK HD``

Die Kartenwerte sind:

* die Zahlen ``2`` bis ``10``
* ``B`` Bube
* ``D`` Dame
* ``K`` König
* ``A`` Ass

Die Kartenfarben sind:

* ``C`` Karo
* ``H`` Herz
* ``P`` Pik
* ``K`` Kreuz

*Obacht: Gegenüber der englischen Kata-Beschreibung haben sich die
 Buchstaben für die Werte und Farben geändert, damit sie den deutschen
 Begriffen entsprechen.  Also nicht wundern, wenn die Karten in einer
 Beispiellösung komisch aussehen – die sind dann wohl englisch.*

## Wertigkeiten

Um die Kata einfach zu halten, sollen nur einzelne Karten (High Card)
oder Paare (Pair) berücksichtig werden.  Jedes Paar ist dabei mehr
wert als eine einzelne Karte.

Die Kartenwerte sind wie oben dargestellt sortiert (die ``2`` ist der
niedrigste, das ``A`` der höchste).

Kartenfarben sind für die Auswertung nicht von Belang.

## Beispiele

* Eingabe ``C8 H3 P9 KB C2`` => Ergebnis ``KB``
* Eingabe ``P3 C5 KB C3 P7`` => Ergebnis ``P3 C3``
