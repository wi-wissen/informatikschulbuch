# ml5.js

ml5.js ist ein Projekt, welches TensorFlow so stark abstrahiert, dass es für KünstlerInnen, Entwickler und Lernende gleichermaßen gut geeignet sein soll.

i> Die vollständige Dokumentation mit vielen Beispielen findest du in einfachem Englisch auf [ml5js.org](https://ml5js.org/).

Die Bibliothek darfst du über den folgenden Link direkt einbinden oder auch herunterladen: https://unpkg.com/ml5

Du musst nur diesen auf deiner Webseite einbinden:

```html
<script src="https://unpkg.com/ml5"></script>
```

i> [**Hier**](https://apps.informatik.cc/neuronale-netze/ml5js/image-classification.html) siehst du ein Beispiel wie Bilder klassifiziert werden können. Das erste Bild ist aus der Trainingsmenge. Das zweite ein zufälliger Mensch, das dritte eine Tasse ud schlussendlich ein zufälliges Foto.

Um ein Foto zu Klassifizieren reicht der folgende Quelltext:

```html
<!DOCTYPE html>
<html>
  <head>
    <head>
      <title>Getting Started with ml5.js</title>
      <script src="https://unpkg.com/ml5"></script>
    </head>

  <body>
    <h1>Image classification using MobileNet</h1>
    <p>The MobileNet model labeled this as
    <span id="result">...</span> with a confidence of
    <span id="probability">...</span></p>
    <img src="https://ml5js.org/docs/assets/img/bird.jpg"
     crossorigin="anonymous" id="image" width="400">

    <script>
      // The image we want to classify
      const image = document.getElementById('image');
      // The result tag in the HTML
      const result = document.getElementById('result');
      // The probability tag in the HTML
      const probability = document.getElementById('probability');

      // Initialize the Image Classifier method with MobileNet
      const classifier = ml5.imageClassifier('MobileNet');

      // Make a prediction with the selected image
      // This will return an array with a default of 10 options with their probabilities
      classifier.predict(image, function(results) {
        result.innerText = results[0].className;
        probability.innerText = results[0].probability.toFixed(4);
      });

    </script>
  </body>
</html>
```

