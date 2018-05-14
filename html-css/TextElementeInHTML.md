# Text-Elemente in HTML

In diesem Abschnitt lernst du die grundlegenden Elemente kennen, die dem Text auf einer Webseite zugewiesen werden können.

## Formatierung

Du kannst Text wie folgt formatieren:

| HTML-Elemente   | Beschreibung  |
| --------------- | ------------- |
| `<b>`Text`</b>` | Fett          |
| `<i>`Text`</i>` | Kursiv        |
| `<u>`Text`</u>` | Unterstrichen |

Sicher fragst du dich, warum der Text keine Farben oder eine andere Schriftart erhalten kann. Um das durchzuführen, lernen wir später CSS.

t> [Aufgabe](https://apps.wi-wissen.de/html-css-js-editor/RKUnQ)

Mehr Elemente zur Formatierung findest du bei [selfhtml.org](https://wiki.selfhtml.org/wiki/HTML/Textauszeichnung)

## Überschriften

Die erste Überschrift hast du schon im vorherigen Abschnitt kennengelernt. Wie in einem Textverarbeitungsprogramm gibt es Überschriften und Unterüberschriften. Dabei ist `Heading 1` die größte Überschrift und `Heading 6` die kleinste Überschrift. Um uns Schreibarbeit zu ersparen, wird `Heading` einfach mit `h` abgekürzt:

```html
<h1>Überschrift 1. Ordnung</h1>
<h2>Überschrift 2. Ordnung</h2>
<h3>Überschrift 3. Ordnung</h3>
<h4>Überschrift 4. Ordnung</h4>
<h5>Überschrift 5. Ordnung</h5>
<h6>Überschrift 6. Ordnung</h6>
```

t> [Aufgabe 1](https://apps.wi-wissen.de/html-css-js-editor/dqe16)

t> [Aufgabe 2](https://apps.wi-wissen.de/html-css-js-editor/WDSWN)

## Zeilenumbrüche

Vielleicht hast du schon bemerkt, dass Eine Webseite den Text nicht umbricht, wenn du die Enter-Taste im Quelltext verwendest. Also verwenden wir ein nichtdruckbares Zeichen, um eine neue Zeile einzuleiten. Da wir das eben nicht schreiben können, verwenden wir ein leeres Element und kürzen dieses ab:

```html
1. Zeile <br /> 2. Zeile
```

i> `br` ist dabei die Abkürzung für break and return



t> [Aufgabe](https://apps.wi-wissen.de/html-css-js-editor/0XtSu)

