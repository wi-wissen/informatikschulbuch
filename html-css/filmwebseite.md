<style type="text/css">
    ol { list-style-type: lower-alpha; }
</style>

# Filmwebseite

In dieser Aufgabe erstellet du eine Webseite zu deinem Lieblingsfilm (oder deiner Lieblingsserie). Du kannst dir einen beliebigen Film von [www.themoviedb.org](http://www.themoviedb.org/) auswählen.

Beispiel: <https://www.themoviedb.org/movie/118340-guardians-of-the-galaxy> 

# 1. Vorbereitung

1. Lade den Ordner `html` [hier](assets/html.zip ':ignore') als zip-Datei herunterladen.

2. Kopiere den Ordner an einen sicheren Speicherort. 
3. Öffne das Programm [Notepad++](https://notepad-plus-plus.org/), [Brackets](http://brackets.io/) oder einen anderen Texteditor aus dem Startmenü
4. Speichere ein leeres Dokument unter dem Dateinamen `index.html` im eben kopierten `html`-Ordner. 

w> Achte darauf, nicht ausversehentlich die Endung `txt` zu verwenden! 

# 2. Inhalt der Webseite

1. Öffne mit Notepad++ die Datei `index.html`

2. Erstelle ein gültiges HTML-Dokument. 

3. Gib im `head ` den Titel des Filmes an. 

4. Schreibe in den `body ` die Filmbeschreibung. (Denke dir diese selbst aus oder kopiere dir diese von [themoviedb.org](https://www.themoviedb.org/).


Expertenaufgabe: Füge in den head noch folgende Befehle ein: 

```html
<link href="css/bootstrap.min.css" rel="stylesheet">
```

## 2.1. Überschrift

1. Füge über der Beschreibung des Films noch den Filmtitel als Überschrift ein. 

2. Nach dem Titel soll in Klammern das Jahr ausgeben werden. Der Text soll dabei kleiner sein, als der der Überschrift. Um einen Text kleiner anzuzeigen, kannst du den `small`-Tag verwenden.


## 2.2. Textformatierung

i> Ein Abschnitt heißt im Englischen „paragraph“. Er wird als `<p></p>` abgekürzt.

1. Erstelle unter dem Filmtitel eine Unterüberschrift mit dem Text „Handlung“

2. Formatiere alle Namen kursiv.

3.  Erstelle unter der Beschreibung einen neuen Abschnitt mit dem Text `Webseite erstellt von Günther`. 

4. Ersetze Günther durch deinen Namen und mache ihn fett. 

5. Schreibe den eben eingefügten Absatz kleiner.


## 2.3. Listen und Tabellen

1. Füge unter der Filmbeschreibung eine geeignete Liste mit 3 wichtigen Genres des Filmes ein.

2. Erstelle eine Tabelle mit 5 wichtigen Schauspielernamen und deren Rollen.

3. Überschreibe Tabelle und Liste mit einer Überschrift. 


Experten: Gib der Tabelle eine Spaltenüberschrift.

## 2.4. Verweise

1. Füge ganz unten auf deiner Seite einen Link zu deinem Film auf [themoviedb.org](https://www.themoviedb.org/) ein. Es soll das Wort Quelle angezeigt werden. 


## 2.5. Bilder und Video

1. Lege im Ordner html einen Ordner img an und speichere darin das Filmposter und ein Filmbackdrop (Bild aus dem Film) ab.

2. Füge das Filmposter nach dem Filmtitel ein. 

i> Nutze dazu wieder [themoviedb.org](https://www.themoviedb.org/)

Expertenaufgabe: 

1. Lege im Ordner `html ` einen Ordner video an und speichere den Trailer für deinen Film ab. 

2. Finde heraus, wie du den Trailer einbinden kannst.

3. Verwende einen Trailer direkt von YouTube.

4. Verwende den Trailer, den du unter `video ` gespeichert hast.


i> Du kannst dazu z.B. auf YouTube gehen und dann den Videolink mit  <http://keepvid.com> speichern. 


# 3. Gestaltung der Webseite

**Ab hier solltest du zuerst CSS aus dem HTML-Tutorial behandelt haben.**

## 3.1. CSS

1. Binde entweder direkt in der Seite oder als extra Datei im Ordner `css ` einen CSS Block ein. 

2. Färbe alle Überschriften in deiner Lieblingsfarbe ein.


## 3.2. Hintergrund

1. Noch ist der Webseitenhintergrund recht fad. 

2. Binde in den Hintergrund ein Backdrop-Bild ein 

Expertenaufgabe: Färbe den Rest des Hintergrundes in einer Kontrastfarbe zu den Überschriften ein.

i> Verwende [background-blend-mode](https://wiki.selfhtml.org/wiki/CSS/Eigenschaften/Hintergrundfarben_und_-bilder/background-blend-mode)

## 3.3. Ausrichten der Webseite

Richte die Elemente mithilfe der Grid-Idee neu aus. Gern kannst du aber auch ein eigenes Layout wählen.

Expertenaufgabe: Gestalte die Filmwebseite nach deinem persönlichen Geschmack. 