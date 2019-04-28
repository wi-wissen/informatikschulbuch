# Elemente in CSS

Bisher sahen unsere Webseiten noch alle sehr gleich aus. Es wird Zeit frischen Wind reinzubringen und unsere Webseiten nach unseren Wünschen zu stylen!

## Grundlagen

Um abweichend vom Browser vorgeschlagenen Aussehen ein anderes zu erreichen, gibt es die CSS-Sprache. Mit dieser wird beschrieben, wie die Webseite aussehen soll:

```html
<h1>grüne Überschrift</h1>
```

```css
h1 {
	color:green;
}
```

t> Gib obiges Beispiel in den [Editor](https://eule27.de/t/C8Z8F) ein.					

In obigen Beispiel wurde die Überschrift anstelle der vom Browser vorgeschlagenen schwarzen Farbe in grün geschrieben.

Dies liegt daran, dass wir in CSS die Eigenschaft `color` mit dem Eigenschaftswert `green` belegt haben. (Da green ein Schlüsselwort ist, muss es nicht, wie in ähnlichen Situationen, in Anführungszeichen gesetzt werden.

Grundsätzlich ist eine HTML-Element-Beschreibung in CSS immer wie folgt aufgebaut:

```css
Element {
	Attribut1: Attributwert1; 
	Attribut2: Attributwert2;
}
```

Nachdem das Element benannt wurde (etwa `body` oder `h1`), wird mit den geschweiften Klammern `{}` Beginn und Ende der Eigenschaften für das Element angezeigt. Mit `Attribut1: Attributwert1` wird dem Attribut1 der Attributwert1 zugewiesen. Das Semikolon `;` beendet die aktuelle Zuweisung und ermöglicht eine weitere.

## Elemente adressieren

In obigen Beispiel haben wir alle Überschriften `h1` grün gefärbt. Oft ist das nicht gewollt und man möchte nur spezielle Elemente ansprechen. Dafür verwenden wir folgende Schreibweise: 

```html
<h1 class="besonders">grüne Überschrift</h1>
```

```css
.besonders {
	color:green;
}
```

Hier werden nur alle Überschriften grün gefärbt, welche bei dem Attribut `class` den Attributwert `besonders` haben.

t> Übernimm das Beispiel in den [Editor](https://eule27.de/t/C8Z8F). 

t> Ändere die Farbe von grün auf rot.

i> Besonders beim Programmieren mit JavaScript ist es wichtig genau ein eindeutiges Element anzusprechen. Dafür verwendet man `<h1 id="top">`, dies spricht man in CSS etwa mit `#top` an. Der Attributwert zu `id` muss auf der gesamten Seite eindeutig sein!



## HTML und CSS zusammenfügen

Um die CSS-Befehle mit dem HTML-Dokument zu verknüpfen, gibt es zwei Möglichkeiten. Beide Möglichkeiten werden im `head` des HTML-Dokumentes umgesetzt, da die Befehle ja nicht angezeigt, sondern ausgeführt werden sollen.

### CSS in HTML einbetten

```html
<style> 
	h1 {
		color:green;
	} 
</style>
```

Hier wird ein HTML-Element namens style im `head`-Bereich des HTML-Dokuments geöffnet. Darin kann CSS geschrieben werden.

Hier ist ein vollständiges Beispiel:

```html
<!DOCTYPE html>
<html>
  <head>
	<meta charset="utf-8">
	<title>Titel der Webseite</title>
    <style> 
      h1 {
          color:green;
      } 
	</style>
	<!-- weitere Kopfinformationen -->
	<!-- Kommentare werden im Browser nicht angezeigt. -->
  </head>
  <body>
	<!-- erst ab hier wird der Inhalt auch im Browser angezeigt. -->
	<h1>grüne Überschrift</h1>
    <p>Inhalt der Webseite</p>
  </body>
</html>
```

t> Erstelle im head deiner Filmwebseite ein CSS-Element.

t> Übernimm darin das Beispiel und prüfe, dass deine Überschriften 1. Grades (`h1`) grün geworden sind. 



## Aus HTML auf CSS verweisen

i> Folgendes Vorgehen ist praktisch, sofern du dein CSS nicht nur auf einer Seite, sondern auf allen Seiten deiner Webseite einbinden möchtest.

```html
<link href="css/style.css" rel="stylesheet">
```

Hier wird für die CSS-Befehle eine extra Datei namens style.css im Unterordner css abgelgt. (Beachte das Kapitel Verweise in HTML!)

