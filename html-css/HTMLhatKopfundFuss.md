# HTML hat Kopf und Fuß

Bisher haben wir immer ein einem Sandkasten unsere ersten Schritte machen können. Nun geht es aber raus auf die Straße!

Eine vollständige Webseite sieht nämlich wie folgt aus:

```html
<!DOCTYPE html>
<html>
  <head>
	<meta charset="utf-8">
    <title>Titel der Webseite</title>
    <!-- weitere Kopfinformationen -->
    <!-- Kommentare werden im Browser nicht angezeigt. -->
  </head>
  <body>
	<!-- erst ab hier wird der Inhalt auch im Browser angezeigt. -->
    <p>Inhalt der Webseite</p>
  </body>
</html>
```

Um das zu verstehen, müssen wir unser gesamtes Wissen zusammennehmen und noch einiges Neue lernen:

Wir haben schon gelernt, dass es Rechtecke gibt, welche wir ineinanderschachteln können. Das ist auch hier der Fall. Es gibt ganz große Rechtecke, von denen wir bisher noch nichts wussten.

`html` - das Rechteck zeigt an, dass es eine HTML-Seite ist. Was du bisher als HTML kennst ist eine Art Dialekt einer größeren Sprache XML (welche wiederum ein Dialekt ist, dazu aber im Informatikstudium mehr)

`head` - dieses Rechteck wird **nicht** im Browserfenster angezeigt. Hier haben wir ganz spezielle Informationen für den Browser abgelegt.

`body` - dieses Rechteck wird im Browserfenster angezeigt und füllt dies vollständig aus.

i> [Hilfe zu Notepad++](https://youtu.be/uuXvdouR-Hw)

t> Öffne Notepad++
t> Kopiere den Text aus dem Beispiel in Notepad++
t> Speichere den Text als "index.html" in deinem H-Laufwerk. Achte  unbedingt darauf, dass kein ".txt" am Ende steht. Ändere dazu die Dateiendung beim Speichern.
t> Öffne dein gespeichertes Dokument im Browser (Doppelklick oder reinziehen).
t> Untersuche, was die Tags p und title bewirken.

s> Glückwunsch! Du kennst nun die Grundlagen von HTML!

t> Wende all dein Wissen und Geschick aus den vorangegangenen Kapiteln auf das Erstellen einer [Filmwebseite](filmwebseite.md) in Aufgabe 1-6 an.