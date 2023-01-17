# Atttribute in CSS

CSS bietet ein Vielzahl an Befehlen. Hier soll dir nur ein Überblick über ausgewählte Befehle gegeben werden. Klickst du auf die Überschrift, kommst du auf [selfhtml.org](https://wiki.selfhtml.org/wiki/CSS), wo du noch viel mehr Befehle findest. Deiner Fantasie sind (fast) keine Grenzen gesetzt!

Im Folgenden findest du zuerst eine Übersicht mit vielen Attributen und Attributwerten.

Danach findest du wichtige Erklärungen zu numerischen Angaben und Farben.

## Übersicht

### [Schriftformatierung](https://wiki.selfhtml.org/wiki/CSS/Eigenschaften/Schriftformatierung)

| Attribut      | Attributwerte                            |
| ------------- | ---------------------------------------- |
| `font-family` | `serif` (Serifenschrift), `sans-serif` (serifenlose Schrift)									Spezielle Schriftnamen gehen auch, diese sind aber nicht auf jeden Rechner installiert (`Times New Roman` nur auf Windows) |
| `font-size`   | `xx-small`, `x-small`, `small`, `medium`, `large`, `x-large`, `xx-large`									numerischer Wert |
| `color`       | Farbe                                    |

t> [Aufgabe](https://eule27.de/t/8Vr8m)

### [Textformatierung](https://wiki.selfhtml.org/wiki/CSS/Eigenschaften/Textformatierung)

| Attribut         | Attributwerte                            |
| ---------------- | ---------------------------------------- |
| `text-transform` | `capitalize`, Wortanfänge als Großbuchstaben, alle anderen Buchstaben werden nicht verändert.<br />`uppercase`, nur Großbuchstaben	<br />`lowercase`, nur Kleinbuchstaben<br />`none`, keine Text-Transformation |

t> [Aufgabe](https://eule27.de/t/G7t89)

### [Textausrichtung](https://wiki.selfhtml.org/wiki/CSS/Eigenschaften/Textausrichtung)

| Attribut     | Attributwerte                            |
| ------------ | ---------------------------------------- |
| `text-align` | `justify` (Blocksatz)<br />`center` (für zentrierte Ausrichtung)<br />`right` (für rechtsbündige Ausrichtung)<br />`left` (für linksbündige Ausrichtung)<br />(gilt auch für Bilder) |

t> [Aufgabe](https://eule27.de/t/M9V8J)

### [äußere Gestaltung](https://wiki.selfhtml.org/wiki/CSS/Eigenschaften/%C3%A4u%C3%9Fere_Gestaltung)

Um hier als Experte agieren zu können, empfiehlt es sich diesen [Artikel](https://wiki.selfhtml.org/wiki/CSS/Box-Modell) schon vorab zu lesen.

| Attribut               | Attributwerte                            |
| ---------------------- | ---------------------------------------- |
| `border-style`         | `none` (kein Rahmen bzw. unsichtbarer Rahmen)<br /> `dotted` (gepunktet)<br /> `dashed` (gestrichelt)<br /> `solid` (durchgezogen)<br /> |
| `border-color`         | Farbe                                    |
| `border-width` | `thin` (dünn),<br /> `medium` (mittelstark),<br /> `thick` (dick)<br /> Numerische Angabe |

t> Wende die obigen Attribute auf den [gegebenen Text](https://eule27.de/t/np2Xo) an.

### [Hintergrundfarben und -bilder](https://wiki.selfhtml.org/wiki/CSS/Eigenschaften/Hintergrundfarben_und_-bilder)

| Attribut           | Attributwerte                          |
| ------------------ | -------------------------------------- |
| `background-image` | `url(`Adresse zum Bild, wie bei img`)` |
| `background-color` | Farbe                                  |

t> Öffne den [Editor](https://eule27.de/t/C8Z8F) und färbe den Hintergrund in deiner Lieblingsfarbe ein.

t> Experten: Probiere eine [RGBA-Farbe](https://wiki.selfhtml.org/wiki/Grafik/Farben#rgba) aus. Was unterscheidet diese von den bisherigen Farben?

Experten: Ein Hintergrundbild wird mit `background-image` festgelegt. Es lassen sich noch deutlich mehr Einstellungen festlegen: 

```css
body {
    background-image: url("../img/backdrop1.jpg");
	background-blend-mode:overlay;
	background-size: 100%;
	background-color: #c2f0f0;
	background-repeat: no-repeat;
	background-position:0px 66px;
	 
}
```

t> Ermittle, was die jeweiligen Attribute bewirken.

### [Animation](https://wiki.selfhtml.org/wiki/CSS/Eigenschaften/Animation)

Dieser Bereich ist für Experten. Hier wird es deutlich komplizierter und rückt teilweise schon stark in die Nähe von Programmierung.

t> Arbeite dich nach eigenen Ermessen in die Thematik ein. Viel Erfolg!

## Farben

Am einfachsten ist es, wenn du den englischen Namen der Farbe kennst, dann kannst du diesen direkt verwenden.

Wie du schon gelernt hast, setzen sich Farben auf dem Bildschirm nach dem RGB-Modell zusammen. Das sind die 3 Grundfarben Rot, Grün und Blau. Jede Grundfarbe kann Werte von `0` bis `255` annehmen (Vielleicht erinnerst du dich sogar, dass 8 Bit als 1 Byte sind.)

i> Farben kannst du dir z.B. mit einem [Color-Picker](http://www.w3schools.com/colors/colors_picker.asp) gut raussuchen.

Die Farbe wird dabei je Grundfarbe angegeben: `rgb(153,68,0)`. Kürzer ist die Angabe `#de5410`, dabei wird die Farbe nicht dezimal, sondern hexadezimal geschrieben (Das #-Zeichen markiert dies) `#RRGGBB` sind dabei die Farben.

i> [Beispiel](https://eule27.de/t/3npzQ)

## numerische Angaben

In HTML-Webseiten gibt es neben festgelegten Größen 3 verschiedene Maßeinheiten:

Zahl in den Einheiten `px` (Pixel), `em` (x-fache Standardschriftgröße), `%` (von der Standardschriftgröße)

i> [Beispiel](https://eule27.de/t/PVxvb)

s> Super! Du hast die Grundlagen in CSS gelegt.

t> Wende all dein Wissen und Geschick aus den vorangegangenen Kapiteln auf das Erstellen einer [Filmwebseite](filmwebseite.md) in Aufgabe 8 und 9 an.