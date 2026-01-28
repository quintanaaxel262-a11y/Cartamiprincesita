<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Para Mi Princesita 💖</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(to right, #ffdde1, #ee9ca7);
      color: #333;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      padding: 20px;
      text-align: center;
    }

    .container {
      background: rgba(255, 255, 255, 0.95);
      padding: 30px;
      border-radius: 15px;
      max-width: 600px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.2);
    }

    h1 {
      color: #e91e63;
      margin-bottom: 20px;
    }

    #letter {
      font-size: 18px;
      line-height: 1.6;
      white-space: pre-wrap;
      min-height: 300px;
    }

    button {
      background-color: #e91e63;
      color: white;
      border: none;
      padding: 12px 25px;
      border-radius: 8px;
      font-size: 16px;
      cursor: pointer;
      margin-top: 20px;
      transition: background 0.3s;
    }

    button:hover {
      background-color: #d81b60;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Mi Princesita 💖</h1>
    <button id="showButton">Leer Carta</button>
    <p id="letter"></p>
  </div>

  <script>
    const button = document.getElementById('showButton');
    const letter = document.getElementById('letter');

    const text = `Mi bebé, mi princesita,

Te escribo porque te amo y porque me duele saber que te lastimé. Sé que te hablé mal y que no te traté como merecés. No quiero justificarme ni minimizar lo que pasó: me equivoqué, y me duele haber sido yo quien te hizo sentir así.

Sé que tengo un carácter difícil y que cuando me enojo no siempre sé parar. A veces hablo sin pensar y termino diciendo cosas que no siento, y eso te lastima. No quiero seguir siendo así con vos. Me duele saber que te hice daño, porque sos la persona que más amo y la que menos merece pasar por eso.

Te trato como mi esposa porque así te siento en mi corazón. Sos mi hogar, mi compañera, mi bebé. Y justamente por eso quiero cambiar. No quiero ser alguien que te hiera, quiero ser alguien que te cuide, que te dé paz y tranquilidad, no miedo ni tristeza.

Perdón, mi princesita. Perdón de verdad. Estoy dispuesto a trabajar en mí, a aprender a controlar lo que siento y a ser mejor para vos, porque vos y lo nuestro valen la pena. Te amo y no quiero perderte por errores que sí puedo corregir.

Con todo mi amor,
Axeelgy`;

    button.addEventListener('click', () => {
      button.style.display = 'none';
      let i = 0;
      const interval = setInterval(() => {
        letter.textContent += text[i];
        i++;
        if(i >= text.length) clearInterval(interval);
      }, 30); // velocidad de escritura
    });
  </script>
</body>
</html>
