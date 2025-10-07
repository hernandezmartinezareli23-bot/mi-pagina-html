# mi-pagina-html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Práctica — Siete datos sobre el Pingüino Emperador</title>
  <meta name="description" content="Práctica de HTML: Siete datos esenciales sobre el pingüino emperador. Ejemplo de estructura semántica, listas y figuras.">
  <style>
    :root{
      --pastel-blue: #a8d8ea;
      --pastel-pink: #fcbad3;
      --muted: #5b6b80;
      --card: #ffffff;
      --radius: 14px;
      font-family: "Poppins", system-ui, -apple-system, "Segoe UI", Roboto, Arial, sans-serif;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      background: linear-gradient(180deg, #f7fbff 0%, #fff 100%);
      color:var(--muted);
      padding:2rem;
    }
    .wrap{
      max-width:900px;
      margin:0 auto;
    }
    header{
      background: linear-gradient(90deg,var(--pastel-blue),var(--pastel-pink));
      color:#fff;
      padding:1rem 1.2rem;
      border-radius:12px;
      box-shadow: 0 8px 20px rgba(16,24,40,0.06);
    }
    header h1{margin:0;font-size:1.3rem}
    header p{margin:0.35rem 0 0;font-weight:300;font-size:0.95rem}
    .content{
      background:var(--card);
      border-radius:var(--radius);
      padding:1.2rem;
      margin-top:1rem;
      box-shadow: 0 8px 20px rgba(16,24,40,0.06);
    }
    .hero{
      display:flex;
      gap:1rem;
      align-items:center;
    }
    .hero img{width:140px;height:auto;border-radius:10px}
    .intro{line-height:1.5}
    ol.facts{
      margin:1rem 0 0;
      padding-left:1.2rem;
    }
    ol.facts li{
      margin:0.9rem 0;
      padding:0.8rem;
      border-radius:10px;
      background: linear-gradient(180deg, #ffffff 0%, #fbfcff 100%);
      border: 1px solid #eef6fb;
    }
    ol.facts li h3{margin:0 0 0.25rem;font-size:1.02rem;color:#152238}
    ol.facts li p{margin:0;font-size:0.95rem;color:var(--muted)}
    .note{
      margin-top:1rem;
      font-size:0.9rem;
      color:#4d6784;
      background:#fbfdff;
      padding:0.7rem;border-radius:10px;border:1px solid #e8f3fb;
    }
    footer{
      margin-top:1rem;text-align:center;font-size:0.9rem;color:#8a9bb3;
    }
    .tema-general{
      text-align:center;
      font-size:2rem;
      font-weight:bold;
      margin-bottom:0.5rem;
      color:#152238;
    }
    .subtema{
      text-align:center;
      font-size:1.2rem;
      font-weight:500;
      margin-bottom:1rem;
      color:#4d6784;
    }
    .imagenes-extra{
      display:flex;
      gap:1rem;
      justify-content:center;
      margin-top:1rem;
      flex-wrap:wrap;
    }
    .imagenes-extra img{
      width:220px;
      border-radius:12px;
      border:2px solid #eef6fb;
    }
    /* Responsive */
    @media (max-width:600px){
      .hero{flex-direction:column;text-align:center}
      .hero img{width:120px}
      .imagenes-extra{flex-direction:column;align-items:center}
    }
  </style>
</head>
<body>
  <div class="wrap">

    <!-- Tema general y subtema -->
    <div class="tema-general">HTML BÁSICO</div>
    <div class="subtema">Estructura de una etiqueta</div>

    <header role="banner" aria-labelledby="title">
      <h1 id="title">Práctica HTML — Siete datos esenciales sobre el Pingüino Emperador</h1>
      <p>Ejercicio: estructura semántica, listas ordenadas y uso de figuras. Tema: pingüinos emperador (cute, tonos pasteles).</p>
    </header>

    <main class="content" role="main">
      <section class="hero" aria-labelledby="hero-title">
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a3/Aptenodytes_forsteri_-Snow_Hill_Island%2C_Antarctica_-adults_and_juvenile-8.jpg/250px-Aptenodytes_forsteri_-Snow_Hill_Island%2C_Antarctica_-adults_and_juvenile-8.jpg" alt="Pingüino emperador adulto de pie en la nieve" width="180" height="180">
        <div>
          <h2 id="hero-title">Conoce a los Pingüinos Emperador</h2>
          <p class="intro">A continuación encontrarás <strong>siete datos esenciales</strong> sobre el pingüino emperador. Este bloque sirve como práctica de estructura HTML (secciones, listas y figuras) y como contenido informativo.</p>
        </div>
      </section>

      <!-- Dos imágenes extra del pingüino emperador -->
      <section class="imagenes-extra">
        <figure>
          <img src="https://ichef.bbci.co.uk/ace/ws/640/cpsprodpb/15C01/production/_106598098_gettyi33758.jpg.webp" alt="Pingüino emperador adulto en la nieve">
          <figcaption>Pingüino emperador en su hábitat natural.</figcaption>
        </figure>
        <figure>
          <img src="data:image/jpeg;base64,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" alt="Pinguinos emperador adultos">
          <figcaption>Cría de pingüino emperador junto a un adulto.</figcaption>
        </figure>
      </section>

      <section aria-labelledby="facts-title" style="margin-top:1rem;">
        <h2 id="facts-title">Siete datos esenciales</h2>
        <ol class="facts">
          <li>
            <h3>1. Los más grandes del mundo</h3>
            <p>Los pingüinos emperadores son las aves pingüino más grandes del planeta: los adultos pueden medir cerca de 1.1 a 1.3 metros de altura.</p>
          </li>
          <li>
            <h3>2. Bucean muy profundo</h3>
            <p>Pueden bucear a mayor profundidad que cualquier otra ave —incluidos otros pingüinos— alcanzando inmersiones largas y profundas en busca de alimento.</p>
          </li>
          <li>
            <h3>3. No construyen nidos</h3>
            <p>En lugar de construir nidos, los pingüinos emperador usan sus patas y los llamados "parches de cría" (colgajos de piel sin plumas) como lugar para mantener y proteger el huevo.</p>
          </li>
          <li>
            <h3>4. Saltan y crean microburbujas</h3>
            <p>Mientras nadan, los emperadores saltan en el aire bajo el agua, lo que los recubre de microburbujas. Esto puede reducir la fricción y posiblemente sea una conducta también asociada al juego.</p>
          </li>
          <li>
            <h3>5. Su "esmoquin" es camuflaje</h3>
            <p>El típico plumaje de esmoquin (vientre blanco y espalda oscura) actúa como camuflaje: el vientre se confunde con la luz desde arriba y la espalda con la oscuridad desde abajo.</p>
          </li>
          <li>
            <h3>6. Reproducción en invierno antártico</h3>
            <p>Son los únicos pingüinos que se reproducen durante el invierno en la Antártida, tolerando condiciones extremadamente frías para incubar sus huevos.</p>
          </li>
          <li>
            <h3>7. Significado del nombre científico</h3>
            <p>El género del pingüino emperador, <em>Aptenodytes</em>, significa literalmente "sin alas — buceador", haciendo referencia a su especialización como nadador.</p>
          </li>
        </ol>

        <aside class="note" aria-label="Nota sobre uso">
          <strong>Práctica recomendada:</strong> transforma cada elemento de la lista en un <code>&lt;article&gt;</code> si quieres practicar estructura semántica avanzada o añade un <code>&lt;details&gt;</code> para mostrar información extra sobre cada dato.
        </aside>
      </section>
    </main>

    <footer role="contentinfo">
      <p>Práctica creada para la serie de HTML/CSS — Tema: Pingüinos Emperador 🐧</p>
    </footer>
  </div>
</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Práctica 3 — Párrafos y Encabezados / Pingüino Emperador</title>
  <style>
    :root {
      --bg: #f5f7fa;
      --card: #ffffff;
      --text: #2c3e50;
      --accent: #2980b9;
      font-family: Arial, sans-serif;
    }
    body {
      background-color: var(--bg);
      color: var(--text);
      margin: 0;
      padding: 1rem;
      line-height: 1.6;
    }
    .wrap {
      max-width: 900px;
      margin: 0 auto;
      background: var(--card);
      padding: 1.5rem;
      border-radius: 8px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    }
    header {
      text-align: center;
      margin-bottom: 1.5rem;
    }
    header h1 {
      color: var(--accent);
      margin-bottom: 0.5rem;
    }
    header p {
      font-style: italic;
      margin: 0;
    }
    h2 {
      color: var(--accent);
      margin-top: 1.5rem;
    }
    h3 {
      margin-top: 1rem;
      color: #34495e;
    }
    p {
      margin-bottom: 1rem;
      text-align: justify;
    }
    .img-section {
      text-align: center;
      margin: 1.5rem 0;
    }
    .img-section img {
      width: 100%;
      max-width: 450px;
      border-radius: 8px;
    }
    footer {
      margin-top: 2rem;
      text-align: center;
      font-size: 0.9rem;
      color: #555;
      border-top: 1px solid #ddd;
      padding-top: 1rem;
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <h1>Práctica 3: Párrafos y Encabezados</h1>
      <p>Ejemplo aplicado al Pingüino Emperador</p>
    </header>

    <div class="img-section">
      <img src="https://static.nationalgeographicla.com/files/styles/image_3200/public/usfws-emperor-penguins_1.webp?w=1600&h=900" alt="Pingüino emperador en la Antártida">
    </div>

    <h2>1. El emperador es la especie de pingüinos más grande del mundo</h2>
    <p>
      Con una altura que ronda entre los 112 y los 115 centímetros y un peso de 22 a 40 kilogramos, esta es la especie más alta y pesada de pingüinos vivos, asegura Global Penguin Society (GPS), una organización reconocida internacionalmente por la conservación de las especies de pingüinos en el mundo.
    </p>
    <p>
      A nivel corporal, los machos son ligeramente más grandes que las hembras, pero se asemejan en plumaje. Ambos tienen la cabeza de color negra, vientre blanco, pecho de color amarillo pálido y manchas auriculares (zona de la oreja) amarillas brillantes, agrega GPS.
    </p>
    <p>
      Al nacer, los ejemplares de <em>Aptenodytes forsteri</em> no tienen plumas, su pelaje es gris y pesan apenas 315 gramos. Las primeras plumas grises aparecen después de semanas de su nacimiento, explica Animal Diversity Web (ADW), una base de datos en línea sobre historia natural de la Universidad de Michigan.
    </p>

    <h2>2. Los pingüinos emperador tienen un hogar muy exclusivo</h2>
    <p>
      Estos ejemplares habitan únicamente en la Antártida, indica ADW. Allí, las temperaturas invernales oscilan entre -40 °C y 0 °C, con una sensación térmica que alcanza los -60 °C.
    </p>
    <p>
      Es la única especie que se reproduce en el invierno antártico, época en la que puede trasladarse entre 50 y 120 kilómetros sobre el hielo para llegar a su colonia de reproducción, donde llegan a encontrarse miles de pingüinos, señala GPS.
    </p>
    <p>
      Durante la temporada de reproducción, las colonias se desplazan a plataformas de hielo. En esos sitios, los acantilados y icebergs les sirven de protección contra los vientos cruzados.
    </p>
    <p>
      Acabada la época de procreación, pasan gran parte del tiempo en áreas de hielo estacionalmente llenas. Estos sitios, cercanos al mar abierto, les permiten acceder fácilmente al alimento, completa ADW.
    </p>

    <h2>3. Mientras las hembras buscan comida, los machos incuban los huevos</h2>
    <p>
      Los pingüinos emperador son ovíparos y tienen un período de incubación que puede durar entre 33 y 62 días, explica un artículo de National Geographic España. Además, detalla GPS, estas aves llegan a la colonia en los meses de marzo-abril, mientras que las hembras ponen un solo huevo entre mayo y junio.
    </p>
    <p>
      Un dato destacado es que las hembras no incuban los huevos, sino que lo hacen los machos, quienes permanecen de pie durante 62 días con el huevo dentro de la bolsa de cría hasta conseguir su objetivo. En ese período, las hembras van al mar para alimentarse.
    </p>
    <p>
      Durante la ausencia de sus parejas, los machos se mantienen en ayuno, lo que puede provocar que pierdan hasta la mitad de su peso corporal, señala el Conicet (Argentina).
    </p>
    <p>
      Cuando nacen las crías, entre finales de julio y comienzos de agosto, las hembras retornan y relevan a los machos, quienes se van al mar abierto para alimentarse y recuperar energías. Luego, los padres se turnan para ir a buscar alimento y cuidar al polluelo, concluye GPS.
    </p>

    <footer>
      <p>Práctica 3 — HTML Básico: Párrafos y Encabezados | Fuente: GPS, ADW, Conicet y National Geographic</p>
    </footer>
  </div>
</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Práctica 4 — Listas en HTML</title>
  <style>
    :root {
      --bg: #f5f7fa;
      --card: #ffffff;
      --text: #2c3e50;
      --accent: #16a085;
      font-family: Arial, sans-serif;
    }
    body {
      background: var(--bg);
      margin: 0;
      padding: 1rem;
      line-height: 1.6;
      color: var(--text);
    }
    .wrap {
      max-width: 900px;
      margin: 0 auto;
      background: var(--card);
      padding: 1.5rem;
      border-radius: 8px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    }
    header {
      text-align: center;
      margin-bottom: 1.5rem;
    }
    header h1 {
      margin: 0;
      color: var(--accent);
    }
    header p {
      margin: 0.5rem 0 0;
      font-style: italic;
    }
    h2 {
      margin-top: 1.5rem;
      color: var(--accent);
    }
    ul, ol {
      margin-left: 1.5rem;
      margin-bottom: 1rem;
    }
    li {
      margin: 0.3rem 0;
    }
    .img-section {
      text-align: center;
      margin: 1.5rem 0;
    }
    .img-section img {
      max-width: 400px;
      width: 100%;
      border-radius: 8px;
    }
    footer {
      margin-top: 2rem;
      text-align: center;
      font-size: 0.9rem;
      color: #555;
      border-top: 1px solid #ddd;
      padding-top: 1rem;
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <h1>Práctica 4: Listas en HTML</h1>
      <p>Ejemplo aplicado al documental <em>La Marche de l'empereur</em></p>
    </header>

    <div class="img-section">
      <img src="https://m.media-amazon.com/images/I/814PR7gEEqL._UF894,1000_QL80_.jpg" alt="Póster de la película La Marche de l'empereur">
    </div>

    <h2>Título</h2>
    <ul>
      <li><strong>España:</strong> El viaje del emperador</li>
      <li><strong>Hispanoamérica:</strong> La marcha de los pingüinos</li>
    </ul>

    <h2>Ficha técnica</h2>
    <ul>
      <li><strong>Dirección:</strong> Luc Jacquet</li>
      <li><strong>Producción:</strong> 
        <ul>
          <li>Ilann Girard</li>
          <li>Yves Darondeau</li>
          <li>Christophe Lioud</li>
          <li>Emmanuel Priou</li>
        </ul>
      </li>
      <li><strong>Guion:</strong> Luc Jacquet, Michel Fessler</li>
      <li><strong>Música:</strong> Emilie Simon</li>
      <li><strong>Fotografía:</strong> Laurent Chalet, Jérôme Maison</li>
      <li><strong>Montaje:</strong> Sabine Emiliani</li>
      <li><strong>Protagonistas:</strong> pingüinos emperador</li>
    </ul>

    <h2>Datos y cifras</h2>
    <ol>
      <li><strong>País:</strong> Francia</li>
      <li><strong>Año:</strong> 2005</li>
      <li><strong>Género:</strong> Documental</li>
      <li><strong>Duración:</strong> 85 minutos</li>
      <li><strong>Idioma(s):</strong> Francés</li>
      <li><strong>Formato:</strong> Película de 16 mm</li>
    </ol>

    <h2>Compañías</h2>
    <ul>
      <li><strong>Productoras:</strong> 
        <ul>
          <li>National Geographic Channel</li>
          <li>Bonne Pioche</li>
          <li>Wild Bunch</li>
          <li>Canal+</li>
          <li>Buena Vista International France</li>
        </ul>
      </li>
      <li><strong>Distribución:</strong>
        <ul>
          <li>Wild Bunch</li>
          <li>Walt Disney Studios Motion Pictures</li>
        </ul>
      </li>
    </ul>

    <h2>Descripción</h2>
    <p>
      <em>La Marche de l'empereur</em> es una película documental francesa dirigida por Luc Jacquet. 
      La película muestra los viajes anuales de los pingüinos emperador de la Antártida. 
    </p>
    <p>
      En otoño, todos los pingüinos en edad reproductiva (más de cinco años) dejan el océano, su hábitat habitual, para iniciar un viaje hacia el interior de la Antártida hacia sus lugares de anidamiento. Allí, los pingüinos comienzan el cortejo que dará lugar a una nueva vida.
    </p>
    <p>
      Durante meses, uno de los padres debe viajar al océano a buscar alimento mientras el otro cuida al polluelo. El rodaje de la película se realizó en los alrededores de la base científica francesa de Dumont d'Urville en Tierra Adelia y duró un año.
    </p>
    <p>
      Incluso se desarrolló un videojuego para la Game Boy Advance titulado <em>March of the Penguins</em>.
    </p>

    <footer>
      <p>Práctica 4 — HTML Básico: Listas | Tema: La Marche de l'empereur 🐧</p>
    </footer>
  </div>
</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Práctica 5 — Enlaces en HTML</title>
  <style>
    :root {
      --bg: #f5f7fa;
      --card: #ffffff;
      --text: #2c3e50;
      --accent: #2980b9;
      font-family: Arial, sans-serif;
    }
    body {
      background: var(--bg);
      margin: 0;
      padding: 1rem;
      line-height: 1.6;
      color: var(--text);
    }
    .wrap {
      max-width: 900px;
      margin: 0 auto;
      background: var(--card);
      padding: 1.5rem;
      border-radius: 8px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    }
    header {
      text-align: center;
      margin-bottom: 1.5rem;
    }
    header h1 {
      margin: 0;
      color: var(--accent);
    }
    header p {
      margin: 0.5rem 0 0;
      font-style: italic;
    }
    h2 {
      margin-top: 1.5rem;
      color: var(--accent);
    }
    a {
      color: var(--accent);
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
    .img-section {
      text-align: center;
      margin: 1.5rem 0;
    }
    .img-section img {
      max-width: 400px;
      width: 100%;
      border-radius: 8px;
    }
    footer {
      margin-top: 2rem;
      text-align: center;
      font-size: 0.9rem;
      color: #555;
      border-top: 1px solid #ddd;
      padding-top: 1rem;
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <h1>Práctica 5 — Enlaces en HTML</h1>
      <p>Subtema: Enlaces básicos</p>
    </header>

    <section>
      <h2>Las mejores películas y documentales con pingüinos</h2>
      <p>
        Descubre nuestra lista de películas y documentales que tienen a los pingüinos como protagonistas, 
        fomentando unos valores positivos en el espectador.
      </p>
      <p>
        Como amantes del pingüino y del cine, hemos querido hacer un recorrido por las películas y documentales 
        en los que los cineastas han querido poner como protagonistas a estos carismáticos animales.
      </p>
      <p>
        Su adorable cara, su forma de caminar o su carácter salvaje y sociable han inspirado obras famosas como 
        <em>Los Pingüinos de Madagascar</em> o el documental <em>La marche de l’empereur</em>.
      </p>
    </section>

    <section>
      <h2>Enlaces a Documentales</h2>
      <ul>
        <li><a href="https://youtu.be/voLMCPDCNk8?si=3IBK1C3L1e1zxwAV">La Marche de l'empereur (YouTube)</a></li>
        <li><a href="https://youtu.be/A9mbCNs47FI?si=nDrUSqHnk8EosSZC"_blank">El reino de los pingüinos (National Geographic)</a></li>
      </ul>
    </section>

    <div class="img-section">
      <img src="https://cdn.milenio.com/uploads/media/2019/11/08/los-pinguino-emperador-podrian-extinguirse_0_21_958_595.jpg" alt="Pingüinos emperador">
    </div>

    <footer>
      <p>Práctica 5 — HTML Básico | Enlaces</p>
    </footer>
  </div>
</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Práctica 6 — Imágenes y Rutas</title>
  <style>
    :root {
      --bg: #f5f7fa;
      --card: #ffffff;
      --text: #2c3e50;
      --accent: #8e44ad;
      font-family: Arial, sans-serif;
    }
    body {
      background: var(--bg);
      margin: 0;
      padding: 1rem;
      line-height: 1.6;
      color: var(--text);
    }
    .wrap {
      max-width: 900px;
      margin: 0 auto;
      background: var(--card);
      padding: 1.5rem;
      border-radius: 8px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    }
    header {
      text-align: center;
      margin-bottom: 1.5rem;
    }
    header h1 {
      margin: 0;
      color: var(--accent);
    }
    header p {
      margin: 0.5rem 0 0;
      font-style: italic;
    }
    h2 {
      margin-top: 1.5rem;
      color: var(--accent);
    }
    ul {
      margin-left: 1.5rem;
      margin-bottom: 1rem;
    }
    li {
      margin: 0.3rem 0;
    }
    .img-section {
      text-align: center;
      margin: 1.5rem 0;
    }
    .img-section img {
      max-width: 400px;
      width: 100%;
      border-radius: 8px;
      margin: 0.5rem;
    }
    footer {
      margin-top: 2rem;
      text-align: center;
      font-size: 0.9rem;
      color: #555;
      border-top: 1px solid #ddd;
      padding-top: 1rem;
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <h1>Práctica 6 — Imágenes y Rutas</h1>
      <p>Subtema: Uso de imágenes en HTML</p>
    </header>

    <section>
      <h2>Pingüino Emperador</h2>
      <p>
        Los pingüinos emperador son los pingüinos más grandes del mundo, alcanzan entre 100 y 122 cm de altura y se reproducen durante el invierno antártico en el hielo marino. 
        Su plumaje blanco y negro les sirve de camuflaje al nadar, y no construyen nidos, sino que el macho incuba el único huevo sobre sus patas. 
        Son capaces de sumergirse más que cualquier otra ave y se alimentan de peces, kril y cefalópodos.
      </p>
    </section>

    <section>
      <h2>Datos curiosos</h2>
      <ul>
        <li><strong>Los más grandes:</strong> hasta 122 cm de altura y 45 kg de peso.</li>
        <li><strong>Reproducción única:</strong> crían en invierno antártico sobre el hielo marino.</li>
        <li><strong>Incubación del macho:</strong> cuida el huevo por 9 semanas sin alimentarse.</li>
        <li><strong>Sin nido:</strong> incuban sobre una bolsa abdominal llamada parche de cría.</li>
        <li><strong>Camuflaje en dos tonos:</strong> blanco por debajo y negro por arriba.</li>
        <li><strong>Nado acrobático:</strong> saltan fuera del agua para nadar más rápido.</li>
        <li><strong>Alimentación profunda:</strong> bucean a grandes profundidades en busca de comida.</li>
        <li><strong>Acurrucamiento:</strong> se agrupan en colonias para protegerse del frío.</li>
        <li><strong>Adaptación al frío:</strong> plumas densas y reservas de grasa.</li>
        <li><strong>Muda catastrófica:</strong> pierden todas sus plumas de golpe en 2-3 semanas.</li>
      </ul>
    </section>

    <section>
      <h2>Ejemplo de Imágenes con Rutas</h2>
      <div class="img-section">
        <!-- Ruta absoluta (imagen desde internet) -->
        <img src="https://cloudfront-us-east-1.images.arcpublishing.com/infobae/3ZEA32SBLNBXRBGMUO24QZVDUA.jpg" alt="Pingüino emperador en la Antártida">

        <!-- Ruta relativa (simulada como si tuvieras una carpeta img en tu proyecto) -->
        <img src="https://ichef.bbci.co.uk/ace/ws/640/cpsprodpb/15C01/production/_106598098_gettyi33758.jpg.webp" alt="Pingüino emperador bebé local (ruta relativa)">
      </div>
    </section>

    <footer>
      <p>Práctica 6 — HTML Básico | Imágenes y Rutas</p>
    </footer>
  </div>
</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Práctica 7 — Formularios en HTML</title>
  <style>
    :root {
      --bg: #f5f7fa;
      --card: #ffffff;
      --text: #2c3e50;
      --accent: #2980b9;
      font-family: Arial, sans-serif;
    }
    body {
      background: var(--bg);
      margin: 0;
      padding: 1rem;
      line-height: 1.6;
      color: var(--text);
    }
    .wrap {
      max-width: 900px;
      margin: 0 auto;
      background: var(--card);
      padding: 1.5rem;
      border-radius: 8px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    }
    header {
      text-align: center;
      margin-bottom: 1.5rem;
    }
    header h1 {
      margin: 0;
      color: var(--accent);
    }
    header p {
      margin: 0.5rem 0 0;
      font-style: italic;
    }
    h2 {
      margin-top: 1.5rem;
      color: var(--accent);
    }
    form {
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }
    label {
      font-weight: bold;
    }
    input, textarea, button {
      padding: 0.6rem;
      border: 1px solid #ccc;
      border-radius: 6px;
      font-size: 1rem;
    }
    button {
      background: var(--accent);
      color: white;
      border: none;
      cursor: pointer;
      transition: 0.3s;
    }
    button:hover {
      background: #1c5d87;
    }
    footer {
      margin-top: 2rem;
      text-align: center;
      font-size: 0.9rem;
      color: #555;
      border-top: 1px solid #ddd;
      padding-top: 1rem;
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <h1>Práctica 7 — Formularios</h1>
      <p>Subtema: Formularios en HTML</p>
    </header>

    <section>
      <h2>¿Quieres saber más sobre los pingüinos emperador?</h2>
      <p>
        Si deseas más información sobre estas increíbles aves, 
        contáctanos en el correo: 
        <strong>hernandez.martinez.areli23@cetis109.edu.mx</strong> 
        o llena el siguiente formulario:
      </p>

      <form>
        <label for="nombre">Nombre:</label>
        <input type="text" id="nombre" name="nombre" placeholder="Escribe tu nombre" required>

        <label for="correo">Correo electrónico:</label>
        <input type="email" id="correo" name="correo" placeholder="ejemplo@email.com" required>

        <label for="mensaje">Mensaje:</label>
        <textarea id="mensaje" name="mensaje" rows="4" placeholder="Escribe tu mensaje aquí..."></textarea>

        <button type="submit">Enviar</button>
      </form>
    </section>

    <footer>
      <p>Práctica 7 — HTML Básico | Formularios</p>
    </footer>
  </div>
</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Práctica — Selectores CSS con pingüinos emperador</title>
  <meta name="description" content="Práctica CSS: uso de selectores básicos con temática de pingüinos emperador.">
  <style>
    :root {
      --pastel-blue: #a8d8ea;
      --pastel-pink: #fcbad3;
      --muted: #5b6b80;
      --card: #ffffff;
      --radius: 14px;
      font-family: "Poppins", system-ui, -apple-system, "Segoe UI", Roboto, Arial, sans-serif;
    }
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }
    body {
      background: linear-gradient(180deg, #f7fbff 0%, #fff 100%);
      color: var(--muted);
      padding: 2rem;
    }
    .wrap {
      max-width: 900px;
      margin: 0 auto;
    }
    header {
      background: linear-gradient(90deg, var(--pastel-blue), var(--pastel-pink));
      color: #fff;
      padding: 1rem 1.2rem;
      border-radius: 12px;
      box-shadow: 0 8px 20px rgba(16,24,40,0.06);
    }
    header h1 {
      margin: 0;
      font-size: 1.3rem;
    }
    header p {
      margin: 0.35rem 0 0;
      font-weight: 300;
      font-size: 0.95rem;
    }
    .tema-general {
      text-align: center;
      font-size: 2rem;
      font-weight: bold;
      margin-bottom: 0.5rem;
      color: #152238;
    }
    .subtema {
      text-align: center;
      font-size: 1.2rem;
      font-weight: 500;
      margin-bottom: 1rem;
      color: #4d6784;
    }
    .content {
      background: var(--card);
      border-radius: var(--radius);
      padding: 1.2rem;
      margin-top: 1rem;
      box-shadow: 0 8px 20px rgba(16,24,40,0.06);
    }

    /* === Selectores CSS que vamos a practicar === */

    /* Selector por etiqueta */
    h2 {
      color: var(--pastel-blue);
      margin-top: 1rem;
      margin-bottom: 0.5rem;
    }

    /* Selector por clase */
    .resaltado {
      background-color: var(--pastel-pink);
      padding: 0.7rem;
      border-radius: 8px;
      border: 1px solid #eecfdf;
      margin: 1rem 0;
    }

    /* Selector por id */
    #alerta {
      color: red;
      font-weight: bold;
      margin-top: 1rem;
    }

    /* Selector compuesto (clase + etiqueta) */
    p.resaltado {
      font-style: italic;
    }

    /* Selector descendiente */
    .content blockquote {
      border-left: 4px solid var(--pastel-blue);
      margin: 1rem 0;
      padding-left: 1rem;
      color: #667788;
    }

  </style>
</head>
<body>
  <div class="wrap">
    <div class="tema-general">CSS BÁSICO</div>
    <div class="subtema">Práctica — Selectores CSS</div>

    <header role="banner" aria-labelledby="title">
      <h1 id="title">Selectores con pingüinos emperador</h1>
      <p>Ejemplo usando selectores de etiquetas, clases, IDs y más</p>
    </header>

    <main class="content" role="main">
      <section>
        <h2>Contexto / Información</h2>
        <p>Según un artículo reportado por la BBC (referencia sobre pingüinos emperador), en una colonia importante hubo una catástrofe reproductiva: miles de polluelos murieron cuando la plataforma de hielo sobre la que vivían se rompió prematuramente. :contentReference[oaicite:0]{index=0}</p>

        <p class="resaltado">Este párrafo está “resaltado” por tener la clase <code>resaltado</code>.</p>

        <h2>Ejemplos de uso de selectores</h2>
        <p>Este es un párrafo normal. Podemos tener otro párrafo <span class="resaltado">resaltado dentro de un texto</span> usando la clase.</p>

        <blockquote>
          “Miles de crías se quedaron sin hielo seguro para desarrollarse antes de poder nadar.”  
        </blockquote>

        <p id="alerta">⚠️ Este texto usa el ID <code>alerta</code>.</p>
      </section>
    </main>

    <footer role="contentinfo">
      <p>Práctica de selectores CSS con temática de pingüinos emperador</p>
    </footer>
  </div>
</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Práctica — Propiedades de texto y fuente</title>
  <meta name="description" content="Práctica CSS: propiedades de texto y fuente con temática de pingüinos emperador.">
  <style>
    :root{
      --pastel-blue: #a8d8ea;
      --pastel-pink: #fcbad3;
      --muted: #5b6b80;
      --card: #ffffff;
      --radius: 14px;
      font-family: "Poppins", system-ui, -apple-system, "Segoe UI", Roboto, Arial, sans-serif;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      background: linear-gradient(180deg, #f7fbff 0%, #fff 100%);
      color:var(--muted);
      padding:2rem;
    }
    .wrap{
      max-width:900px;
      margin:0 auto;
    }
    header{
      background: linear-gradient(90deg,var(--pastel-blue),var(--pastel-pink));
      color:#fff;
      padding:1rem 1.2rem;
      border-radius:12px;
      box-shadow: 0 8px 20px rgba(16,24,40,0.06);
    }
    header h1{margin:0;font-size:1.3rem}
    header p{margin:0.35rem 0 0;font-weight:300;font-size:0.95rem}
    .content{
      background:var(--card);
      border-radius:var(--radius);
      padding:1.2rem;
      margin-top:1rem;
      box-shadow: 0 8px 20px rgba(16,24,40,0.06);
    }
    .tema-general{
      text-align:center;
      font-size:2rem;
      font-weight:bold;
      margin-bottom:0.5rem;
      color:#152238;
    }
    .subtema{
      text-align:center;
      font-size:1.2rem;
      font-weight:500;
      margin-bottom:1rem;
      color:#4d6784;
    }

    /* ==== PROPIEDADES DE TEXTO Y FUENTE ==== */
    .ejemplo1 {
      font-size: 1.4rem; 
      font-weight: bold;
      text-transform: uppercase;
      text-align: center;
      color: #152238;
    }
    .ejemplo2 {
      font-style: italic;
      text-decoration: underline;
      letter-spacing: 2px;
      color: var(--pastel-blue);
    }
    .ejemplo3 {
      line-height: 2;
      word-spacing: 8px;
      font-family: "Courier New", monospace;
      color: var(--pastel-pink);
    }
    .ejemplo4 {
      text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
      font-size: 1.2rem;
      font-weight: 600;
      color: #34495e;
    }
    .ejemplo5 {
      font-variant: small-caps;
      background: #fef6fb;
      padding: 0.5rem;
      border-radius: 8px;
      display: inline-block;
    }
    footer{
      margin-top:1rem;text-align:center;font-size:0.9rem;color:#8a9bb3;
    }
  </style>
</head>
<body>
  <div class="wrap">
    <div class="tema-general">CSS BÁSICO</div>
    <div class="subtema">Práctica — Propiedades de texto y fuente</div>

    <header role="banner" aria-labelledby="title">
      <h1 id="title">Texto y Fuente en CSS</h1>
      <p>Ejemplos aplicados a frases sobre pingüinos emperador</p>
    </header>

    <main class="content">
      <p class="ejemplo1">El pingüino emperador es el más grande de todos.</p>
      <p class="ejemplo2">Los machos incuban el huevo durante semanas sin comer.</p>
      <p class="ejemplo3">Su plumaje blanco y negro es un camuflaje perfecto en el océano.</p>
      <p class="ejemplo4">Son capaces de bucear a más de 500 metros de profundidad.</p>
      <p class="ejemplo5">En grupo, se acurrucan para resistir el frío antártico.</p>
    </main>

    <footer role="contentinfo">
      <p>Práctica CSS — Propiedades de texto y fuente</p>
    </footer>
  </div>
</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Práctica — Tipografías externas</title>
  <meta name="description" content="Práctica de HTML y CSS: Uso de tipografías externas aplicadas en frases sobre el pingüino emperador.">
  
  <!-- Importamos tipografías de Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Lobster&family=Raleway:wght@300;500;700&display=swap" rel="stylesheet">

  <style>
    :root{
      --pastel-blue: #a8d8ea;
      --pastel-pink: #fcbad3;
      --muted: #5b6b80;
      --card: #ffffff;
      --radius: 14px;
      font-family: "Raleway", system-ui, Arial, sans-serif;
    }

    *{box-sizing:border-box}
    body{
      margin:0;
      background: linear-gradient(180deg, #f7fbff 0%, #fff 100%);
      color:var(--muted);
      padding:2rem;
    }

    .wrap{ max-width:900px; margin:0 auto; }

    header{
      background: linear-gradient(90deg,var(--pastel-blue),var(--pastel-pink));
      color:#fff;
      padding:1rem 1.2rem;
      border-radius:12px;
      box-shadow: 0 8px 20px rgba(16,24,40,0.06);
    }
    header h1{margin:0;font-size:1.6rem;font-family:"Lobster", cursive;}
    header p{margin:0.35rem 0 0;font-weight:300;font-size:0.95rem}

    .content{
      background:var(--card);
      border-radius:var(--radius);
      padding:1.2rem;
      margin-top:1rem;
      box-shadow: 0 8px 20px rgba(16,24,40,0.06);
    }

    .tema-general{
      text-align:center;
      font-size:2rem;
      font-weight:bold;
      margin-bottom:0.5rem;
      color:#152238;
      font-family:"Lobster", cursive;
    }

    .subtema{
      text-align:center;
      font-size:1.2rem;
      font-weight:500;
      margin-bottom:1rem;
      color:#4d6784;
    }

    .texto1{
      font-family:"Raleway", sans-serif;
      font-weight:300;
      font-size:1.1rem;
      margin:1rem 0;
    }
    .texto2{
      font-family:"Raleway", sans-serif;
      font-weight:500;
      font-size:1.2rem;
      color:#152238;
      margin:1rem 0;
    }
    .texto3{
      font-family:"Lobster", cursive;
      font-size:1.5rem;
      color:#e85a92;
      margin:1rem 0;
    }

    .imagenes-extra{
      display:flex;
      gap:1rem;
      justify-content:center;
      margin-top:1rem;
    }
    .imagenes-extra img{
      width:200px;
      border-radius:12px;
      border:2px solid #eef6fb;
    }

    footer{ margin-top:1rem;text-align:center;font-size:0.9rem;color:#8a9bb3; }

    /* Responsive */
    @media (max-width:600px){
      .imagenes-extra{flex-direction:column;align-items:center}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <h1>Práctica — Tipografías externas</h1>
      <p>Ejemplo con frases sobre el Pingüino Emperador 🐧</p>
    </header>

    <main class="content">
      <div class="tema-general">Pingüino Emperador</div>
      <div class="subtema">Tipografías externas en acción</div>

      <p class="texto1">🌊 El pingüino emperador puede sumergirse hasta 500 metros en busca de alimento.</p>
      <p class="texto2">❄️ Es la única especie que se reproduce durante el invierno antártico.</p>
      <p class="texto3">👑 El emperador de los hielos resiste temperaturas extremas bajo cero.</p>

      <div class="imagenes-extra">
        <img src="https://static.nationalgeographicla.com/files/styles/image_3200/public/nationalgeographic_1528132.jpg?w=1600" alt="Pareja de Pingüinos emperador con su cría">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS39qRKcNvZq2x8g8iznrqILxwdiM-2HmYECA&s" alt="Colonia de pingüinos emperador">
      </div>
    </main>

    <footer>
      Práctica CSS — Tipografías externas | CETis 109
    </footer>
  </div>
</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Práctica — Modelo de Caja (Box Model)</title>
  <meta name="description" content="Práctica de HTML y CSS: Modelo de caja aplicado en frases sobre el pingüino emperador.">
  <style>
    :root{
      --pastel-blue: #a8d8ea;
      --pastel-pink: #fcbad3;
      --muted: #5b6b80;
      --card: #ffffff;
      --radius: 14px;
      font-family: "Poppins", system-ui, -apple-system, "Segoe UI", Roboto, Arial, sans-serif;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      background: linear-gradient(180deg, #f7fbff 0%, #fff 100%);
      color:var(--muted);
      padding:2rem;
    }
    .wrap{ max-width:900px; margin:0 auto; }
    header{
      background: linear-gradient(90deg,var(--pastel-blue),var(--pastel-pink));
      color:#fff;
      padding:1rem 1.2rem;
      border-radius:12px;
      box-shadow: 0 8px 20px rgba(16,24,40,0.06);
    }
    header h1{margin:0;font-size:1.6rem}
    header p{margin:0.35rem 0 0;font-weight:300;font-size:0.95rem}
    .content{
      background:var(--card);
      border-radius:var(--radius);
      padding:1.2rem;
      margin-top:1rem;
      box-shadow: 0 8px 20px rgba(16,24,40,0.06);
    }
    .tema-general{
      text-align:center;
      font-size:2rem;
      font-weight:bold;
      margin-bottom:0.5rem;
      color:#152238;
    }
    .subtema{
      text-align:center;
      font-size:1.2rem;
      font-weight:500;
      margin-bottom:1rem;
      color:#4d6784;
    }

    /* Ejemplos de Box Model */
    .box{
      margin:1rem 0;
      padding:1rem;
      border:3px solid var(--pastel-blue);
      border-radius:12px;
      background:#fff;
      box-shadow: 0 4px 10px rgba(0,0,0,0.05);
    }
    .box h3{ margin-top:0; color:#152238; }
    .box p{ margin:0.4rem 0 0; font-size:0.95rem; }

    /* Variaciones para mostrar el modelo de caja */
    .box.padding{
      padding:2rem;
      border-color: var(--pastel-pink);
    }
    .box.margin{
      margin:2rem;
      border-style: dashed;
    }
    .box.borde{
      border:5px dotted #fca4b3;
      background:#fef7fa;
    }

    .imagenes-extra{
      display:flex;
      gap:1rem;
      justify-content:center;
      margin-top:1rem;
    }
    .imagenes-extra img{
      width:200px;
      border-radius:12px;
      border:2px solid #eef6fb;
    }

    footer{ margin-top:1rem;text-align:center;font-size:0.9rem;color:#8a9bb3; }

    /* Responsive */
    @media (max-width:600px){
      .imagenes-extra{flex-direction:column;align-items:center}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <h1>Práctica — Modelo de Caja (Box Model)</h1>
      <p>Ejemplo aplicado a frases sobre el Pingüino Emperador 🐧</p>
    </header>

    <main class="content">
      <div class="tema-general">Pingüino Emperador</div>
      <div class="subtema">Ejemplos del Modelo de Caja</div>

      <div class="box">
        <h3>Altura y resistencia</h3>
        <p>El pingüino emperador puede medir más de 1 metro de altura y soportar temperaturas extremas.</p>
      </div>

      <div class="box padding">
        <h3>Buceo impresionante</h3>
        <p>Puede bucear hasta 500 metros gracias a su capacidad pulmonar y resistencia física.</p>
      </div>

      <div class="box margin">
        <h3>Cría en invierno</h3>
        <p>Es la única especie de pingüino que se reproduce durante el invierno antártico.</p>
      </div>

      <div class="box borde">
        <h3>Colaboración social</h3>
        <p>Los pingüinos emperador se agrupan en círculos para conservar el calor corporal.</p>
      </div>

      <div class="imagenes-extra">
        <img src="https://i.pinimg.com/736x/8e/58/69/8e58691b6f3b2e4ebc081f35f7383238.jpg"Pingüino emperador en la nieve">
        <img src="https://www.24morelos.com/content/images/wp-content/uploads/2019/04/pinguWEB.jpg" alt="Colonia de pingüinos emperador">
      </div>
    </main>

    <footer>
      Práctica CSS — Modelo de Caja | CETis 109
    </footer>
  </div>
</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Práctica — Margen y Relleno con Pingüinos Emperador</title>
  <meta name="description" content="Práctica de HTML y CSS: Relleno y Margen (margin y padding) aplicados en tarjetas con información sobre el pingüino emperador."> 
  <style>
    :root{
      --pastel-blue: #a8d8ea;
      --pastel-pink: #fcbad3;
      --muted: #5b6b80;
      --card: #ffffff;
      --radius: 14px;
      font-family: "Poppins", system-ui, Arial, sans-serif;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      background: linear-gradient(180deg, #f7fbff 0%, #fff 100%);
      color:var(--muted);
      padding:2rem;
    }
    .wrap{
      max-width:900px;
      margin:0 auto;
    }
    header{
      background: linear-gradient(90deg,var(--pastel-blue),var(--pastel-pink));
      color:#fff;
      padding:1rem 1.2rem;
      border-radius:12px;
      text-align:center;
      box-shadow: 0 8px 20px rgba(16,24,40,0.06);
    }
    header h1{margin:0;font-size:1.5rem}
    header p{margin:0.35rem 0 0;font-weight:300;font-size:1rem}
    
    .content{
      background:var(--card);
      border-radius:var(--radius);
      padding:1.2rem;
      margin-top:1rem;
      box-shadow: 0 8px 20px rgba(16,24,40,0.06);
    }

    .ejemplo{
      margin:1rem 0;
      padding:1rem;
      background: linear-gradient(180deg, #ffffff 0%, #fbfcff 100%);
      border:1px solid #eef6fb;
      border-radius:10px;
    }
    .ejemplo h3{
      margin:0 0 0.5rem;
      font-size:1.1rem;
      color:#152238;
    }
    .ejemplo p{margin:0;font-size:0.95rem}

    /* Ejemplos prácticos */
    .margen-grande{
      margin:2rem; /* más separación hacia afuera */
    }
    .padding-grande{
      padding:2rem; /* más espacio interno */
    }
    .margen-vs-padding{
      margin:1.5rem;
      padding:2rem;
    }

    .imagenes-extra{
      display:flex;
      gap:1rem;
      justify-content:center;
      margin-top:1rem;
    }
    .imagenes-extra img{
      width:200px;
      border-radius:12px;
      border:2px solid #eef6fb;
    }

    footer{
      margin-top:1rem;
      text-align:center;
      font-size:0.9rem;
      color:#8a9bb3;
    }

    /* Responsive */
    @media (max-width:600px){
      .imagenes-extra{flex-direction:column;align-items:center}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <h1>Práctica — Margen y Relleno</h1>
      <p>Aplicado con información de los Pingüinos Emperador 🐧</p>
    </header>

    <div class="content">
      <div class="ejemplo margen-grande">
        <h3>Ejemplo de margen</h3>
        <p>Este bloque tiene un <b>margen externo amplio</b>.  
        Representa la distancia que dejan los pingüinos al caminar en grupo sobre el hielo.</p>
      </div>

      <div class="ejemplo padding-grande">
        <h3>Ejemplo de relleno (padding)</h3>
        <p>Este bloque tiene un <b>espacio interno amplio</b>.  
        Como el espacio dentro de los pliegues donde los pingüinos protegen a sus crías del frío.</p>
      </div>

      <div class="ejemplo margen-vs-padding">
        <h3>Margen + Relleno</h3>
        <p>Aquí combinamos <b>margen y padding</b> para mostrar cómo el espacio interno y externo se aplican al mismo tiempo.</p>
      </div>

      <div class="imagenes-extra">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSm7myOlyV0qkFxVzV45Gg75v7c36d34nMaZg&s" alt="Grupo de pingüinos emperador">
        <img src="https://cdn.milenio.com/uploads/media/2019/11/08/los-pinguino-emperador-podrian-extinguirse_0_21_958_595.jpg" alt="Pingüino emperador protegiendo a su cría">
      </div>
    </div>

    <footer>
      Práctica CSS — Margen y Relleno ✨
    </footer>
  </div>
</body>
</html>

<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Práctica — Margen y Relleno con Pingüinos Emperador</title>
  <meta name="description" content="Práctica de HTML y CSS: margen y relleno aplicados en tarjetas con información sobre el pingüino emperador.">
  <style>
    :root{
      --pastel-blue: #a8d8ea;
      --pastel-pink: #fcbad3;
      --muted: #5b6b80;
      --card: #ffffff;
      --radius: 14px;
      font-family: "Poppins", system-ui, Arial, sans-serif;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      background: linear-gradient(180deg, #f7fbff 0%, #fff 100%);
      color:var(--muted);
      padding:2rem;
    }
    .wrap{
      max-width:900px;
      margin:0 auto;
    }
    header{
      background: linear-gradient(90deg,var(--pastel-blue),var(--pastel-pink));
      color:#fff;
      padding:1rem 1.2rem;
      border-radius:12px;
      text-align:center;
      box-shadow: 0 8px 20px rgba(16,24,40,0.06);
    }
    header h1{margin:0;font-size:1.5rem}
    header p{margin:0.35rem 0 0;font-weight:300;font-size:1rem}
    
    .content{
      background:var(--card);
      border-radius:var(--radius);
      padding:1.2rem;
      margin-top:1rem;
      box-shadow: 0 8px 20px rgba(16,24,40,0.06);
    }

    .ejemplo{
      margin:1rem 0;
      padding:1rem;
      background: linear-gradient(180deg, #ffffff 0%, #fbfcff 100%);
      border:1px solid #eef6fb;
      border-radius:10px;
    }
    .ejemplo h3{
      margin:0 0 0.5rem;
      font-size:1.1rem;
      color:#152238;
    }
    .ejemplo p{margin:0;font-size:0.95rem}

    .imagenes-extra{
      display:flex;
      gap:1rem;
      justify-content:center;
      margin-top:1rem;
    }
    .imagenes-extra img{
      width:200px;
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Práctica — Bordes con Pingüinos Emperador</title>
  <meta name="description" content="Práctica de HTML y CSS: Bordes aplicados en tarjetas con información sobre el pingüino emperador."> 
  <style>
    :root{
      --pastel-blue: #a8d8ea;
      --pastel-pink: #fcbad3;
      --muted: #5b6b80;
      --card: #ffffff;
      --radius: 14px;
      font-family: "Poppins", system-ui, Arial, sans-serif;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      background: linear-gradient(180deg, #f7fbff 0%, #fff 100%);
      color:var(--muted);
      padding:2rem;
    }
    .wrap{
      max-width:900px;
      margin:0 auto;
    }
    header{
      background: linear-gradient(90deg,var(--pastel-blue),var(--pastel-pink));
      color:#fff;
      padding:1rem 1.2rem;
      border-radius:12px;
      text-align:center;
      box-shadow: 0 8px 20px rgba(16,24,40,0.06);
    }
    header h1{margin:0;font-size:1.5rem}
    header p{margin:0.35rem 0 0;font-weight:300;font-size:1rem}
    
    .content{
      background:var(--card);
      border-radius:var(--radius);
      padding:1.2rem;
      margin-top:1rem;
      box-shadow: 0 8px 20px rgba(16,24,40,0.06);
    }

    .ejemplo{
      margin:1rem 0;
      padding:1rem;
      background: linear-gradient(180deg, #ffffff 0%, #fbfcff 100%);
      border-radius:10px;
    }
    .ejemplo h3{
      margin:0 0 0.5rem;
      font-size:1.1rem;
      color:#152238;
    }
    .ejemplo p{margin:0;font-size:0.95rem}

    /* Bordes variados */
    .borde-solido{
      border: 3px solid var(--pastel-blue);
    }
    .borde-punteado{
      border: 3px dotted var(--pastel-pink);
    }
    .borde-dashed{
      border: 3px dashed #a6b1e1;
    }
    .borde-redondeado{
      border: 3px solid #84a9ac;
      border-radius: 20px;
    }

    .imagenes-extra{
      display:flex;
      gap:1rem;
      justify-content:center;
      margin-top:1rem;
    }
    .imagenes-extra img{
      width:200px;
      border-radius:12px;
      border:2px solid #eef6fb;
    }

    footer{
      margin-top:1rem;
      text-align:center;
      font-size:0.9rem;
      color:#8a9bb3;
    }

    /* Responsive */
    @media (max-width:600px){
      .imagenes-extra{flex-direction:column;align-items:center}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <h1>Práctica de Bordes</h1>
      <p>Ejemplo aplicado a los Pingüinos Emperador 🐧</p>
    </header>

    <div class="content">
      <div class="ejemplo borde-solido">
        <h3>Borde sólido</h3>
        <p>Este bloque usa un <b>borde sólido</b> en azul pastel.  
        Representa la solidez de las colonias de pingüinos en el hielo.</p>
      </div>

      <div class="ejemplo borde-punteado">
        <h3>Borde punteado</h3>
        <p>Este bloque usa un <b>borde punteado</b> en rosa pastel.  
        Como las huellas de los pingüinos en la nieve.</p>
      </div>

      <div class="ejemplo borde-dashed">
        <h3>Borde discontinuo (dashed)</h3>
        <p>Este bloque usa un <b>borde discontinuo</b>.  
        Representa las trayectorias en zigzag que siguen al nadar.</p>
      </div>

      <div class="ejemplo borde-redondeado">
        <h3>Borde redondeado</h3>
        <p>Este bloque tiene un <b>borde redondeado</b> con esquinas curvas.  
        Como el contorno suave de los cuerpos de los pingüinos emperador.</p>
      </div>

      <div class="imagenes-extra">
        <img src="https://preview.redd.it/s1bu7yok2r951.jpg?auto=webp&s=8517d35e43401279fc48c7b3e186a2b1cb50a5c3" alt="Pingüinos emperador en grupo">
        <img src="https://content.nationalgeographic.com.es/medio/2019/01/19/aptenodytes-forsteri_2c39daac_1280x851.jpg" alt="Pingüino emperador con su cría">
      </div>
    </div>

    <footer>
      Práctica CSS — Bordes 
    </footer>
  </div>
</body>
</html>
<div class="wrap">
  <!-- Sección existente... -->

  <!-- NUEVA SECCIÓN AISLADA -->
  <div class="content">
    <div class="subtema">Sección Aislada — Tamaño de Caja</div>
    
    <p class="intro">Esta sección demuestra <strong>box-sizing</strong> aplicado solo aquí, sin afectar otros elementos del sitio.</p>
    
    <div class="ejemplo-seccion">
      <p>Pingüino Emperador caminando (content-box)</p>
    </div>

    <div class="ejemplo-seccion" style="box-sizing: border-box;">
      <p>Pingüino Emperador cuidando su cría (border-box)</p>
    </div>
    
    <div class="note">
      Nota: Aquí usamos una clase nueva <strong>.ejemplo-seccion</strong> para no modificar las demás tarjetas.
    </div>
  </div>
</div>

<style>
  /* Estilos específicos para la sección aislada */
  .ejemplo-seccion {
    margin: 1rem 0;
    padding: 1rem;
    width: 300px;
    height: 120px;
    background: linear-gradient(180deg, #ffffff 0%, #fbfcff 100%);
    border: 1px solid #eef6fb;
    border-radius: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
  }

  /* Si quieres, puedes añadir más estilos específicos aquí solo para esta sección */
</style>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Práctica — Colores con Pingüinos Emperador</title>
  <meta name="description" content="Práctica de HTML y CSS: Colores aplicados en tarjetas con información sobre el pingüino emperador."> 
  <style>
    :root{
      --pastel-blue: #a8d8ea;
      --pastel-pink: #fcbad3;
      --muted: #5b6b80;
      --card: #ffffff;
      --radius: 14px;
      font-family: "Poppins", system-ui, Arial, sans-serif;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      background: linear-gradient(180deg, #f7fbff 0%, #fff 100%);
      color:var(--muted);
      padding:2rem;
    }
    .wrap{
      max-width:900px;
      margin:0 auto;
    }
    header{
      background: linear-gradient(90deg,var(--pastel-blue),var(--pastel-pink));
      color:#fff;
      padding:1rem 1.2rem;
      border-radius:12px;
      text-align:center;
      box-shadow
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Práctica — Sección Aislada sobre Pingüinos Emperador</title>
  <meta name="description" content="Práctica de HTML y CSS: Sección aislada de colores y tarjetas con información sobre el pingüino emperador.">
  <style>
    :root{
      --pastel-blue: #a8d8ea;
      --pastel-pink: #fcbad3;
      --muted: #5b6b80;
      --card: #ffffff;
      --radius: 14px;
      font-family: "Poppins", system-ui, Arial, sans-serif;
    }
    * { box-sizing: border-box; }
    body {
      margin:0;
      background: linear-gradient(180deg, #f7fbff 0%, #fff 100%);
      color: var(--muted);
      padding: 2rem;
    }
    .wrap { max-width: 900px; margin:0 auto; }

    header {
      background: linear-gradient(90deg,var(--pastel-blue),var(--pastel-pink));
      color: #fff;
      padding: 1rem 1.2rem;
      border-radius: 12px;
      text-align: center;
      box-shadow: 0 8px 20px rgba(16,24,40,0.06);
    }
    header h1 { margin:0; font-size:1.5rem; }
    header p { margin:0.35rem 0 0; font-weight:300; font-size:1rem; }

    /* Estilos generales de contenido */
    .content{
      background: var(--card);
      border-radius: var(--radius);
      padding:1.2rem;
      margin-top:1rem;
      box-shadow: 0 8px 20px rgba(16,24,40,0.06);
    }

    .ejemplo{
      margin:1rem 0;
      padding:1rem;
      background: linear-gradient(180deg, #ffffff 0%, #fbfcff 100%);
      border:1px solid #eef6fb;
      border-radius:10px;
    }
    .ejemplo h3 { margin:0 0 0.5rem; font-size:1.1rem; color:#152238; }
    .ejemplo p { margin:0; font-size:0.95rem; }

    .imagenes-extra{
      display:flex;
      gap:1rem;
      justify-content:center;
      margin-top:1rem;
    }
    .imagenes-extra img{
      width:200px;
      border-radius:12px;
      border:2px solid #eef6fb;
    }

    /* NUEVA SECCIÓN AISLADA */
    .seccion-aislada {
      background: #f0f8ff;
      padding: 1rem;
      margin-top: 2rem;
      border-radius: 12px;
      border: 1px dashed #a8d8ea;
    }
    .seccion-aislada .tarjeta {
      background: #ffffff;
      padding: 1rem;
      margin: 1rem 0;
      border-radius: 10px;
      border: 1px solid #eef6fb;
    }
    .seccion-aislada .tarjeta h4 {
      margin:0 0 0.5rem;
      color:#152238;
    }
    .seccion-aislada .tarjeta p {
      margin:0;
      font-size:0.95rem;
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <h1>Pingüinos Emperador</h1>
      <p>Sección aislada de práctica sobre colores y tarjetas</p>
    </header>

    <!-- Nueva sección aislada -->
    <div class="seccion-aislada">
      <h2 class="subtema">Sección Aislada — Información de los polluelos</h2>

      <div class="tarjeta">
        <h4>Nacimiento</h4>
        <p>Los polluelos de pingüino emperador nacen en uno de los lugares más inhóspitos de la Tierra: el mundo helado de la Antártida.</p>
      </div>

      <div class="tarjeta">
        <h4>Aprendizaje</h4>
        <p>Tras unos cinco meses, los padres abandonan a sus crías. Los juveniles aprenden a nadar, bucear y encontrar comida por sí mismos.</p>
      </div>

      <div class="tarjeta">
        <h4>Supervivencia</h4>
        <p>Los investigadores colocaron rastreadores para registrar movimientos y comportamiento bajo el hielo, observando inmersiones de hasta 264 metros.</p>
      </div>
    </div>
  </div>
</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Prácticas de CSS — Pingüinos Emperador</title>

  <style>
    /* ==== ESTILOS GENERALES ==== */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #e6f4f9;
      color: #03344d;
    }

    h2 {
      text-align: center;
      margin-top: 40px;
    }

    section {
      padding: 20px;
      border-top: 2px solid #a2d2ff;
    }

    .contenedor {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-wrap: wrap;
      gap: 20px;
      margin-top: 20px;
    }

    /* ==== 1️⃣ TAMAÑO DE CAJA (BOX-SIZING) ==== */
    .box {
      width: 150px;
      height: 150px;
      background-color: #90e0ef;
      border: 5px solid #03045e;
      padding: 20px;
      color: white;
      text-align: center;
    }

    .contenido {
      box-sizing: content-box; /* por defecto */
    }

    .borde {
      box-sizing: border-box;
      background-color: #0077b6;
    }

    /* ==== 2️⃣ COLORES ==== */
    .color {
      width: 100px;
      height: 100px;
      border-radius: 10px;
      border: 2px solid #000;
    }

    .color1 { background-color: rgb(0, 119, 182); }
    .color2 { background-color: #ffd60a; }
    .color3 { background-color: hsl(200, 70%, 50%); }

    /* ==== 3️⃣ UNIDADES ==== */
    .unidades p {
      font-size: 1.5em; /* relativo al tamaño del body */
    }

    .unidades .caja {
      width: 50%;
      height: 100px;
      background-color: #caf0f8;
      border: 2px solid #0077b6;
      text-align: center;
      line-height: 100px;
      margin: 10px auto;
    }

    /* ==== 4️⃣ FONDOS, GRADIENTES Y SOMBRAS ==== */
    .fondos {
      background: linear-gradient(to right, #0096c7, #48cae4);
      color: white;
      padding: 40px;
      text-align: center;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
    }

    .fondos img {
      width: 200px;
      border-radius: 50%;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
      border: 5px solid white;
    }

    /* ==== 5️⃣ EJERCICIO PRÁCTICO ==== */
    .tarjeta {
      width: 250px;
      background-color: white;
      border-radius: 15px;
      box-shadow: 0 5px 10px rgba(0, 0, 0, 0.3);
      overflow: hidden;
      text-align: center;
      transition: transform 0.3s;
    }

    .tarjeta:hover {
      transform: scale(1.05);
    }

    .tarjeta img {
      width: 100%;
      height: 150px;
      object-fit: cover;
    }

    .tarjeta h3 {
      color: #023e8a;
      margin: 10px 0;
    }

    .tarjeta p {
      padding: 0 15px 15px;
      font-size: 0.9em;
    }
  </style>
</head>
<body>

  <!-- 1️⃣ Tamaño de caja -->
  <section>
    <h2>1️⃣ Tamaño de Caja (box-sizing)</h2>
    <div class="contenedor">
      <div class="box contenido">content-box</div>
      <div class="box borde">border-box</div>
    </div>
  </section>

  <!-- 2️⃣ Colores -->
  <section>
    <h2>2️⃣ Colores</h2>
    <div class="contenedor">
      <div class="color color1"></div>
      <div class="color color2"></div>
      <div class="color color3"></div>
    </div>
  </section>

  <!-- 3️⃣ Unidades -->
  <section class="unidades">
    <h2>3️⃣ Unidades</h2>
    <p>Ejemplo de unidades relativas y absolutas</p>
    <div class="caja">Ancho: 50%</div>
  </section>

  <!-- 4️⃣ Fondos, Gradientes y Sombras -->
  <section class="fondos">
    <h2>4️⃣ Fondos, Gradientes y Sombras</h2>
    <p>Los pingüinos emperador viven en la Antártida y resisten bajas temperaturas.</p>
    <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTK4XiqBG8DR62LCfbf7ybOrGlt7NymDuTqEcUoUULsqVN2SNXehJy5u-HbTOJ4sUWi_2g&usqp=CAU" alt="Pingüino emperador" />
  </section>

  <!-- 5️⃣ Ejercicio práctico -->
  <section>
    <h2>5️⃣ Ejercicio Práctico</h2>
    <div class="contenedor">
      <div class="tarjeta">
        <img src="https://www.estrategia-sustentable.com.mx/wp-content/uploads/2023/05/NickySouness-9260-1132x509.jpg" alt="Pingüino bebé">
        <h3>Pingüino Emperador</h3>
        <p>El pingüino emperador es la especie más grande. Puede medir hasta 1.2 m y soportar temperaturas extremas.</p>
      </div>
      <div class="tarjeta">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRSWW5pNGma7L4AK4souHyxoqa8zorK0T4kvQ&s" alt="Pingüinos adultos">
        <h3>Su hábitat</h3>
        <p>Viven en colonias y se agrupan para protegerse del frío durante los inviernos antárticos.</p>
      </div>
    </div>
  </section>

</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <!-- 🐧 1️⃣ METATAGS, COMENTARIOS E ICONOS -->
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Prácticas de HTML sobre pingüinos emperador — Curso completo">
  <meta name="author" content="Estudiante de Programación">
  <link rel="icon" href="https://upload.wikimedia.org/wikipedia/commons/3/3e/Emperor_Penguin_Manchot_empereur.jpg" type="image/x-icon">
  <title>Prácticas de HTML — Pingüinos Emperador</title>

  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background-color: #e8f6fa;
      color: #03344d;
    }

    h1 {
      text-align: center;
      font-size: 2.5em;
      margin-top: 20px;
    }

    section {
      padding: 30px;
      border-top: 3px solid #0077b6;
    }

    h2 {
      font-size: 1.8em;
      color: #03045e;
      margin-bottom: 10px;
      border-left: 6px solid #00b4d8;
      padding-left: 10px;
    }

    textarea, input, select {
      padding: 5px;
      margin: 5px 0;
      width: 250px;
      display: block;
    }

    table {
      border-collapse: collapse;
      width: 80%;
      margin: 10px auto;
    }

    th, td {
      border: 2px solid #0096c7;
      padding: 8px;
      text-align: center;
    }

    th {
      background-color: #caf0f8;
    }

    img {
      width: 250px;
      border-radius: 10px;
      display: block;
      margin: 10px auto;
    }

    audio, video {
      display: block;
      margin: 15px auto;
      border-radius: 10px;
    }

    summary {
      cursor: pointer;
      font-weight: bold;
    }

    a {
      color: #0077b6;
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    .obsoleto {
      background-color: #ffd6a5;
      padding: 10px;
      border-radius: 10px;
    }

    article, section, footer, header, nav {
      margin-bottom: 10px;
      padding: 10px;
      border-radius: 10px;
      background-color: #f6f9fc;
    }

    footer {
      text-align: center;
      background-color: #03045e;
      color: white;
      padding: 15px;
    }
  </style>
</head>

<body>
  <h1>🐧 Prácticas de HTML — Basadas en el Curso</h1>

  <!-- 🅰️ 1. Metatags, Comentarios e Iconos -->
  <section>
    <h2>🅰️ 1. Metatags, Comentarios e Iconos</h2>
    <!-- Este es un comentario en HTML -->
    <p>Esta sección usa metatags en el encabezado para definir idioma, autor, descripción y un ícono de pingüino 🐧.</p>
  </section>

  <!-- 🅱️ 2. Textarea y Labels -->
  <section>
    <h2>🅱️ 2. Textarea y Labels</h2>
    <label for="comentario">¿Qué opinas sobre los pingüinos emperador?</label>
    <textarea id="comentario" rows="4" cols="50" placeholder="Escribe tu respuesta aquí..."></textarea>
  </section>

  <!-- 🅲️ 3. Select, Datalist y Option -->
  <section>
    <h2>🅲️ 3. Select, Datalist y Option</h2>
    <label for="color">Selecciona el color del plumaje del pingüino:</label>
    <select id="color">
      <option>Negro</option>
      <option>Blanco</option>
      <option>Gris</option>
      <option>Amarillo</option>
    </select>

    <label for="comida">¿Qué comida prefieren?</label>
    <input list="alimentos" id="comida" placeholder="Ejemplo: Pescado">
    <datalist id="alimentos">
      <option value="Pescado">
      <option value="Calamar">
      <option value="Krill">
    </datalist>
  </section>

  <!-- 🅳 4. Fieldset y Legend -->
  <section>
    <h2>🅳 4. Fieldset y Legend</h2>
    <fieldset>
      <legend>Información del pingüino</legend>
      <label>Nombre: <input type="text" placeholder="Ej. Pingo" /></label>
      <label>Edad: <input type="number" placeholder="Ej. 5" /></label>
    </fieldset>
  </section>

  <!-- 🅴 5. Details y Summary -->
  <section>
    <h2>🅴 5. Details y Summary</h2>
    <details>
      <summary>Información sobre el pingüino emperador</summary>
      <p>El pingüino emperador es la especie más grande y vive exclusivamente en la Antártida.</p>
    </details>
  </section>

  <!-- 🅵 6. Enlaces (Avanzado) -->
  <section>
    <h2>🅵 6. Enlaces (Avanzado)</h2>
    <p>Visita el <a href="https://es.wikipedia.org/wiki/Ping%C3%BCino_emperador" target="_blank">artículo de Wikipedia</a> sobre los pingüinos emperador.</p>
    <a href="#final">Ir al final de la página</a>
  </section>

  <!-- 🅶 7. Tablas -->
  <section>
    <h2>🅶 7. Tablas</h2>
    <table>
      <tr>
        <th>Etapa</th>
        <th>Descripción</th>
      </tr>
      <tr>
        <td>Huevo</td>
        <td>El macho lo incuba sobre sus patas.</td>
      </tr>
      <tr>
        <td>Polluelo</td>
        <td>Se mantiene cálido bajo el plumaje del padre.</td>
      </tr>
    </table>
  </section>

  <!-- 🅷 8. Audio y Video -->
  <section>
    <h2>🅷 8. Audio y Video</h2>
    <audio controls>
      <source src="https://media.istockphoto.com/id/472603355/video/antarctic-penguin-colony-medium-shot.mp4?s=mp4-640x640-is&k=20&c=k35ULCBsuqLPkhdiX4no4cp-iKw1nk4am-3d-JwBP3A=" type="audio/mpeg">
      Tu navegador no soporta audio.
    </audio>
    <video controls width="320">
      <source src="https://media.istockphoto.com/id/472603355/video/antarctic-penguin-colony-medium-shot.mp4?s=mp4-640x640-is&k=20&c=k35ULCBsuqLPkhdiX4no4cp-iKw1nk4am-3d-JwBP3A=" type="video/mp4">
      Tu navegador no soporta video.
    </video>
  </section>

  <!-- 🅸 9. Lazy Loading -->
  <section>
    <h2>🅸 9. Lazy Loading</h2>
    <img loading="lazy" src="https://static.wikia.nocookie.net/reinoanimalia/images/d/d9/Padre_y_cria.jpg/revision/latest/scale-to-width-down/340?cb=20130226212138&path-prefix=es" alt="Pingüinos emperadores">
    <p>La imagen se carga solo cuando se muestra en pantalla (lazy loading).</p>
  </section>

  <!-- 🅹 10. HTML Obsoleto -->
  <section>
    <h2>🅹 10. HTML Obsoleto</h2>
    <div class="obsoleto">
      <p><b>Ejemplo:</b> Las etiquetas <code>&lt;center&gt;</code> y <code>&lt;font&gt;</code> ya no se deben usar.</p>
    </div>
  </section>

  <!-- 🅺 11. HTML Semántico -->
  <section>
    <h2>🅺 11. HTML Semántico</h2>
    <header>Encabezado principal de la página</header>
    <nav>Menú de navegación (Inicio | Galería | Contacto)</nav>
    <article>Artículo sobre la vida de los pingüinos emperador</article>
    <aside>Dato curioso: pueden bucear más de 500 metros.</aside>
    <footer>Pie de página con derechos reservados</footer>
  </section>

  <!-- 🅻 12. Accesibilidad WEB -->
  <section id="final">
    <h2>🅻 12. Accesibilidad WEB</h2>
    <p>Incluye atributos como <code>alt</code> en imágenes y etiquetas <code>label</code> para mejorar la accesibilidad.</p>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a3/Aptenodytes_forsteri_-Snow_Hill_Island%2C_Antarctica_-adults_and_juvenile-8.jpg/500px-Aptenodytes_forsteri_-Snow_Hill_Island%2C_Antarctica_-adults_and_juvenile-8.jpg" alt="Pingüino emperador de pie">
  </section>

  <footer>
    <p>© 2025 Proyecto educativo — Conservación en Acción 🐧</p>
  </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>🐧 Prácticas CSS Intermedio — Pingüinos Emperador</title>

  <style>
    /* 🎨 ESTILOS GENERALES */
    body {
      font-family: "Poppins", sans-serif;
      margin: 0;
      background-color: #fef6ff;
      color: #003049;
    }

    h1 {
      text-align: center;
      font-size: 2.5em;
      background: linear-gradient(to right, #90e0ef, #ffc8dd);
      color: #03045e;
      padding: 20px;
      border-bottom: 5px solid #a2d2ff;
    }

    section {
      padding: 30px;
      margin: 20px;
      border-radius: 15px;
      background-color: #fff0f5;
      border: 3px solid #a2d2ff;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    }

    h2 {
      font-size: 1.8em;
      color: #4361ee;
      border-left: 8px solid #ffafcc;
      padding-left: 10px;
      margin-bottom: 15px;
    }

    /* 1️⃣ Selectores Avanzados */
    .selectores p {
      color: #03045e;
    }
    .selectores p:first-child {
      color: #ff4d6d;
      font-weight: bold;
    }
    .selectores p:nth-child(3) {
      background-color: #caffbf;
    }

    /* 2️⃣ Herencia, Cascada y Especificidad */
    .herencia {
      color: #0077b6;
    }
    .herencia strong {
      color: #ff4d6d; /* más específico */
    }

    /* 3️⃣ Pseudoclases */
    .pseudoclases a {
      color: #0077b6;
      text-decoration: none;
      font-weight: bold;
    }
    .pseudoclases a:hover {
      color: #ff4d6d;
    }
    .pseudoclases a:active {
      color: #03045e;
    }

    /* 4️⃣ Pseudoelementos */
    .pseudoelemento::first-line {
      color: #ff4d6d;
      font-weight: bold;
    }

    /* 5️⃣ Metodología BEM */
    .tarjeta {
      background-color: #caf0f8;
      border-radius: 10px;
      padding: 15px;
      width: 200px;
    }
    .tarjeta__titulo {
      color: #03045e;
      font-weight: bold;
    }
    .tarjeta__texto {
      color: #0077b6;
    }
    .tarjeta--destacada {
      border: 3px solid #ff4d6d;
    }

    /* 6️⃣ Display */
    .display {
      display: flex;
      justify-content: center;
      gap: 15px;
    }
    .display div {
      width: 100px;
      height: 100px;
      background-color: #90e0ef;
      border-radius: 10px;
    }

    /* 7️⃣ Posición Relativa y Absoluta */
    .relativo {
      position: relative;
      background-color: #a2d2ff;
      height: 150px;
    }
    .absoluto {
      position: absolute;
      top: 40px;
      left: 40px;
      background-color: #ffafcc;
      padding: 10px;
      border-radius: 10px;
    }

    /* 8️⃣ Ventanas Modal */
    .fondo-modal {
      display: none;
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: rgba(0,0,0,0.5);
      justify-content: center;
      align-items: center;
    }
    .modal {
      background-color: white;
      padding: 20px;
      border-radius: 10px;
      width: 250px;
      text-align: center;
    }

    /* 9️⃣ Posición Fixed y Sticky */
    .barra {
      position: sticky;
      top: 0;
      background-color: #0077b6;
      color: white;
      padding: 10px;
      text-align: center;
      border-radius: 10px;
    }

    /* 🔟 Transiciones */
    .transicion div {
      width: 100px;
      height: 100px;
      background-color: #ffc8dd;
      transition: all 0.5s;
      border-radius: 10px;
    }
    .transicion div:hover {
      background-color: #0077b6;
      transform: scale(1.2);
    }

    /* 11️⃣ Desbordamiento */
    .overflow {
      width: 250px;
      height: 100px;
      overflow: auto;
      background-color: #caf0f8;
      padding: 10px;
      border: 2px solid #0077b6;
    }

    /* 12️⃣ Control de flujo del texto */
    .flujo {
      width: 200px;
      white-space: nowrap;
      overflow: hidden;
      text-overflow: ellipsis;
      border: 2px solid #ffafcc;
      padding: 10px;
    }

    /* 13️⃣ Object-fit y Object-position */
    .objeto img {
      width: 200px;
      height: 150px;
      object-fit: cover;
      object-position: top;
      border-radius: 10px;
    }

    /* 14️⃣ Contorno (outline) */
    .outline button {
      border: none;
      padding: 10px 20px;
      background-color: #90e0ef;
      outline: 3px solid #ff4d6d;
      border-radius: 10px;
    }

    /* 15️⃣ Emmet */
    .emmet {
      display: flex;
      justify-content: center;
      gap: 10px;
    }
    .emmet div {
      background-color: #ffc8dd;
      width: 100px;
      height: 100px;
      border-radius: 15px;
    }

    button {
      background-color: #ff4d6d;
      color: white;
      border: none;
      padding: 10px 15px;
      border-radius: 8px;
      cursor: pointer;
    }

    button:hover {
      background-color: #03045e;
    }
  </style>
</head>
<body>

  <h1>🐧 Prácticas CSS Intermedio — Colores Rosa y Azul</h1>

  <!-- 1️⃣ Selectores (Avanzado) -->
  <section class="selectores">
    <h2>1️⃣ Selectores (Avanzado)</h2>
    <p>El pingüino emperador vive en la Antártida.</p>
    <p>Es la especie más grande de todas.</p>
    <p>Su plumaje lo protege del frío extremo.</p>
  </section>

  <!-- 2️⃣ Herencia, Cascada y Especificidad -->
  <section class="herencia">
    <h2>2️⃣ Herencia, Cascada y Especificidad</h2>
    <p>Este texto hereda el color azul, pero <strong>este texto tiene prioridad y es rosa</strong>.</p>
  </section>

  <!-- 3️⃣ Pseudoclases -->
  <section class="pseudoclases">
    <h2>3️⃣ Pseudoclases</h2>
    <a href="#">Pasa el cursor o haz clic aquí 🐧</a>
  </section>

  <!-- 4️⃣ Pseudoelementos -->
  <section>
    <h2>4️⃣ Pseudoelementos</h2>
    <p class="pseudoelemento">Los pingüinos cuidan sus huevos sobre sus patas para evitar que se congelen.</p>
  </section>

  <!-- 5️⃣ Metodología BEM -->
  <section>
    <h2>5️⃣ Metodología BEM</h2>
    <div class="tarjeta tarjeta--destacada">
      <p class="tarjeta__titulo">Pingüino Emperador</p>
      <p class="tarjeta__texto">Ejemplo con BEM: bloque, elemento y modificador.</p>
    </div>
  </section>

  <!-- 6️⃣ Display -->
  <section>
    <h2>6️⃣ Display</h2>
    <div class="display">
      <div></div>
      <div></div>
      <div></div>
    </div>
  </section>

  <!-- 7️⃣ Posición Relativa y Absoluta -->
  <section>
    <h2>7️⃣ Posición Relativa y Absoluta</h2>
    <div class="relativo">
      <div class="absoluto">Soy absoluto</div>
    </div>
  </section>

  <!-- 8️⃣ Ventanas Modal -->
  <section>
    <h2>8️⃣ Ventanas Modal</h2>
    <button onclick="document.querySelector('.fondo-modal').style.display='flex'">Abrir Modal</button>
    <div class="fondo-modal">
      <div class="modal">
        <p>🐧 ¡Hola! Soy una ventana modal.</p>
        <button onclick="document.querySelector('.fondo-modal').style.display='none'">Cerrar</button>
      </div>
    </div>
  </section>

  <!-- 9️⃣ Posición Fixed y Sticky -->
  <section>
    <h2>9️⃣ Posición Fixed y Sticky</h2>
    <div class="barra">Soy una barra Sticky 💙</div>
    <p>Desplázate hacia abajo y verás que la barra se mantiene fija.</p>
  </section>

  <!-- 🔟 Transiciones -->
  <section class="transicion">
    <h2>🔟 Transiciones</h2>
    <div></div>
  </section>

  <!-- 11️⃣ Desbordamiento (overflow) -->
  <section>
    <h2>11️⃣ Desbordamiento (Overflow)</h2>
    <div class="overflow">
      Los pingüinos emperador pueden bucear hasta 500 metros bajo el hielo para buscar alimento. Su cuerpo está adaptado para soportar grandes presiones submarinas.
    </div>
  </section>

  <!-- 12️⃣ Control de flujo del texto -->
  <section>
    <h2>12️⃣ Control de flujo del texto</h2>
    <div class="flujo">Este texto es muy largo y se corta con puntos suspensivos...</div>
  </section>

  <!-- 13️⃣ Object Fit y Position -->
  <section class="objeto">
    <h2>13️⃣ Object Fit y Object Position</h2>
    <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRdWAh6-v2spXXA9sa7ByrFUGqV2ZFqX10m8g&s" alt="Pingüinos emperador">
  </section>

  <!-- 14️⃣ Contorno -->
  <section class="outline">
    <h2>14️⃣ Contorno (Outline)</h2>
    <button>Contorno rosa 💗</button>
  </section>

  <!-- 15️⃣ Emmet -->
  <section class="emmet">
    <h2>15️⃣ Emmet (Material reusado)</h2>
    <div></div>
    <div></div>
    <div></div>
  </section>

</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Prácticas CSS FLEXBOX - Pingüinos Emperador</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: linear-gradient(to bottom right, #f9c5d1, #a1c4fd);
      margin: 0;
      padding: 0;
      color: #333;
    }

    h1 {
      text-align: center;
      background-color: #ffb6c1;
      color: #003366;
      padding: 20px;
      margin: 0;
    }

    section {
      margin: 30px;
      padding: 20px;
      background-color: white;
      border-radius: 15px;
      box-shadow: 0 0 10px rgba(0,0,0,0.2);
    }

    section h2 {
      font-size: 24px;
      color: #003366;
      border-bottom: 3px solid #ff66b2;
      padding-bottom: 5px;
    }

    /* 1. Introducción a Flexbox */
    .flex-intro {
      display: flex;
      gap: 10px;
      background-color: #e0f7fa;
      padding: 10px;
    }

    .flex-intro div {
      background-color: #ffccf9;
      padding: 20px;
      text-align: center;
      border-radius: 10px;
      flex: 1;
    }

    /* 2. Flex Direction, Wrap y Flow */
    .flex-direction {
      display: flex;
      flex-direction: row-reverse;
      flex-wrap: wrap;
      gap: 10px;
      background-color: #e3f2fd;
      padding: 10px;
    }

    .flex-direction div {
      background-color: #f8bbd0;
      padding: 20px;
      border-radius: 10px;
    }

    /* 3. Alineación en los ejes */
    .alineacion {
      display: flex;
      justify-content: space-around;
      align-items: center;
      height: 150px;
      background-color: #b3e5fc;
    }

    .alineacion div {
      background-color: #ffb6c1;
      padding: 15px;
      border-radius: 10px;
    }

    /* 4. Order */
    .order {
      display: flex;
      gap: 10px;
    }

    .order div {
      background-color: #c5cae9;
      padding: 15px;
      border-radius: 10px;
    }

    .order div:nth-child(2) {
      order: -1;
    }

    /* 5. Flex Basis, Grow y Shrink */
    .flex-grow {
      display: flex;
    }

    .flex-grow div {
      background-color: #f48fb1;
      margin: 5px;
      padding: 15px;
      flex-basis: 100px;
      flex-grow: 1;
      flex-shrink: 1;
      border-radius: 10px;
    }

    /* 6. Align Self */
    .align-self {
      display: flex;
      align-items: flex-start;
      background-color: #bbdefb;
      height: 200px;
    }

    .align-self div {
      background-color: #f8bbd0;
      margin: 10px;
      padding: 15px;
      border-radius: 10px;
    }

    .align-self div:nth-child(2) {
      align-self: center;
    }

    .align-self div:nth-child(3) {
      align-self: flex-end;
    }

    /* 7. Layout con Flexbox */
    .layout {
      display: flex;
      flex-direction: row;
      gap: 20px;
    }

    .menu {
      background-color: #f48fb1;
      flex: 1;
      padding: 15px;
      border-radius: 10px;
    }

    .contenido {
      background-color: #e1f5fe;
      flex: 3;
      padding: 15px;
      border-radius: 10px;
    }

    .aside {
      background-color: #ce93d8;
      flex: 1;
      padding: 15px;
      border-radius: 10px;
    }
  </style>
</head>
<body>
  <h1>🐧 Prácticas CSS FLEXBOX - Pingüinos Emperador 🐧</h1>

  <section>
    <h2>1️⃣ Introducción a Flexbox</h2>
    <div class="flex-intro">
      <div>Pingüino A</div>
      <div>Pingüino B</div>
      <div>Pingüino C</div>
    </div>
    <p>Los pingüinos jóvenes aprenden a coordinar sus movimientos mientras nadan juntos, similar a cómo los elementos se organizan en un contenedor Flexbox.</p>
  </section>

  <section>
    <h2>2️⃣ Flex Direction, Wrap y Flow</h2>
    <div class="flex-direction">
      <div>Elemento 1</div>
      <div>Elemento 2</div>
      <div>Elemento 3</div>
      <div>Elemento 4</div>
    </div>
    <p>La dirección y el flujo de los pingüinos nadando recuerdan cómo Flexbox distribuye los elementos en diferentes direcciones.</p>
  </section>

  <section>
    <h2>3️⃣ Alineación en los Ejes</h2>
    <div class="alineacion">
      <div>Izquierda</div>
      <div>Centro</div>
      <div>Derecha</div>
    </div>
    <p>Los pingüinos se alinean de forma natural cuando cazan, igual que los elementos en un eje principal y cruzado.</p>
  </section>

  <section>
    <h2>4️⃣ Order</h2>
    <div class="order">
      <div>1</div>
      <div>2 (adelantado)</div>
      <div>3</div>
    </div>
    <p>Algunos pingüinos toman la delantera, cambiando el orden natural como en Flexbox con la propiedad <code>order</code>.</p>
  </section>

  <section>
    <h2>5️⃣ Flex Basis, Grow y Shrink</h2>
    <div class="flex-grow">
      <div>🐧</div>
      <div>🐧🐧</div>
      <div>🐧🐧🐧</div>
    </div>
    <p>Así como los pingüinos crecen a diferentes ritmos, los elementos pueden expandirse o contraerse con <code>flex-grow</code> y <code>flex-shrink</code>.</p>
  </section>

  <section>
    <h2>6️⃣ Align Self</h2>
    <div class="align-self">
      <div>Inicio</div>
      <div>Centro</div>
      <div>Final</div>
    </div>
    <p>Cada pingüino puede posicionarse de forma individual, igual que los elementos con la propiedad <code>align-self</code>.</p>
  </section>

  <section>
    <h2>7️⃣ Layout con Flexbox</h2>
    <div class="layout">
      <div class="menu">Menú</div>
      <div class="contenido">
        <h3>Cómo aprenden los pingüinos</h3>
        <p>Los jóvenes pingüinos emperadores aprenden a nadar, bucear y encontrar comida por sí mismos al dejar la colonia. Los rastreadores satelitales permitieron registrar más de 62.000 inmersiones, mostrando su aprendizaje y desplazamiento en busca de aguas cálidas y comida.</p>
      </div>
      <div class="aside">Publicidad / Información</div>
    </div>
  </section>

</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Prácticas Responsive Design - Pingüinos Emperador</title>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      background: linear-gradient(to bottom right, #f9c5d1, #a1c4fd);
      color: #333;
      margin: 0;
      padding: 0;
    }

    h1 {
      text-align: center;
      background-color: #ffb6c1;
      color: #003366;
      padding: 20px;
      margin: 0;
    }

    section {
      background-color: white;
      margin: 25px;
      padding: 20px;
      border-radius: 15px;
      box-shadow: 0 0 10px rgba(0,0,0,0.2);
    }

    section h2 {
      font-size: 24px;
      color: #003366;
      border-bottom: 3px solid #ff66b2;
      padding-bottom: 5px;
    }

    img, video {
      max-width: 100%;
      border-radius: 10px;
    }

    /* 1️⃣ Bloques y Multimedia flexible */
    .flexible {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }

    .flexible div {
      flex: 1 1 300px;
      background-color: #e1f5fe;
      padding: 10px;
      border-radius: 10px;
    }

    /* 2️⃣ Atributos SRCSET y SIZES */
    picture, img {
      width: 100%;
      border-radius: 10px;
    }

    /* 4️⃣ Media Queries */
    .media {
      display: flex;
      flex-direction: row;
      gap: 20px;
    }

    .media div {
      flex: 1;
      background-color: #f8bbd0;
      padding: 15px;
      border-radius: 10px;
    }

    @media (max-width: 800px) {
      .media {
        flex-direction: column;
      }
    }

    /* 5️⃣ Holy Grail con Flexbox */
    .holy {
      display: flex;
      flex-direction: row;
      gap: 10px;
    }

    .menu {
      background-color: #f48fb1;
      flex: 1;
      padding: 15px;
      border-radius: 10px;
    }

    .contenido {
      background-color: #e1f5fe;
      flex: 3;
      padding: 15px;
      border-radius: 10px;
    }

    .aside {
      background-color: #ce93d8;
      flex: 1;
      padding: 15px;
      border-radius: 10px;
    }

    @media (max-width: 800px) {
      .holy {
        flex-direction: column;
      }
    }

    /* 6️⃣ Mobile First */
    .mobile {
      display: flex;
      flex-direction: column;
    }

    @media (min-width: 700px) {
      .mobile {
        flex-direction: row;
      }
      .mobile div {
        flex: 1;
      }
    }

    .mobile div {
      background-color: #bbdefb;
      margin: 10px;
      padding: 15px;
      border-radius: 10px;
    }

    /* 7️⃣ Feature Queries */
    @supports (display: grid) {
      .feature {
        display: grid;
        grid-template-columns: 1fr 1fr;
      }
    }

    .feature div {
      background-color: #e1bee7;
      padding: 15px;
      border-radius: 10px;
      margin: 5px;
    }

    /* 8️⃣ Container Queries (simulada) */
    .container {
      border: 2px solid #003366;
      padding: 15px;
      max-width: 600px;
      margin: auto;
      border-radius: 15px;
      background-color: #f0f4ff;
    }

    .container p {
      font-size: 18px;
    }

    @container (max-width: 500px) {
      .container p {
        font-size: 14px;
        color: #ff4081;
      }
    }
  </style>
</head>
<body>
  <h1>🐧 Prácticas RESPONSIVE DESIGN - Pingüinos Emperador 🐧</h1>

  <section>
    <h2>1️⃣ Bloques y Multimedia flexible</h2>
    <div class="flexible">
      <div>
        <p>Los jóvenes pingüinos aprenden a nadar y bucear de forma independiente, adaptándose a los cambios de su entorno.</p>
      </div>
      <div>
        <img src="https://content.nationalgeographic.com.es/medio/2019/01/19/aptenodytes-forsteri_2c39daac_1280x851.jpg" alt="Pingüinos Emperador">
      </div>
    </div>
  </section>

  <section>
    <h2>2️⃣ Atributos SRCSET y SIZES</h2>
    <picture>
      <source srcset="https://upload.wikimedia.org/wikipedia/commons/5/54/Emperor_Penguin_Manchot_empereur.jpg" media="(min-width: 800px)">
      <source srcset="https://upload.wikimedia.org/wikipedia/commons/9/96/Emperor_penguin_chick.jpg" media="(min-width: 400px)">
      <img src="https://content.nationalgeographic.com.es/medio/2019/01/19/aptenodytes-forsteri_2c39daac_1280x851.jpg" alt="Pingüinos adaptándose al clima">
    </picture>
    <p>Con <code>srcset</code> y <code>sizes</code> las imágenes cambian según el tamaño de la pantalla, igual que los pingüinos se adaptan a su entorno.</p>
  </section>

  <section>
    <h2>3️⃣ Picture, Source y Media</h2>
    <picture>
      <source srcset="https://upload.wikimedia.org/wikipedia/commons/4/4c/Emperor_penguin_Antarctica.jpg" media="(min-width:800px)">
      <source srcset="https://upload.wikimedia.org/wikipedia/commons/9/96/Emperor_penguin_chick.jpg" media="(min-width:400px)">
      <img src="https://content.nationalgeographic.com.es/medio/2019/01/19/aptenodytes-forsteri_2c39daac_1280x851.jpg" alt="Pingüinos emperadores">
    </picture>
    <p>El uso de <code>picture</code> y <code>source</code> permite mostrar distintas imágenes según el ancho de la pantalla.</p>
  </section>

  <section>
    <h2>4️⃣ Media Queries</h2>
    <div class="media">
      <div>Pingüinos en grupo</div>
      <div>Adaptación al frío</div>
    </div>
    <p>Las <code>@media queries</code> ajustan el diseño como los pingüinos ajustan su comportamiento según la temperatura.</p>
  </section>

  <section>
    <h2>5️⃣ Ejercicio “Holy Grail” con Flexbox</h2>
    <div class="holy">
      <div class="menu">Menú</div>
      <div class="contenido">
        <h3>Cómo aprenden los pingüinos</h3>
        <p>Los rastreadores satelitales mostraron que los pingüinos jóvenes se mueven al norte, aprenden a nadar y luego regresan al hielo marino en invierno.</p>
      </div>
      <div class="aside">Información adicional</div>
    </div>
  </section>

  <section>
    <h2>6️⃣ Mobile First</h2>
    <div class="mobile">
      <div>Etapa 1: Aprenden a nadar</div>
      <div>Etapa 2: Aprenden a bucear</div>
      <div>Etapa 3: Encuentran alimento</div>
    </div>
    <p>El diseño <strong>Mobile First</strong> comienza desde pantallas pequeñas, creciendo como los pingüinos en su desarrollo.</p>
  </section>

  <section>
    <h2>7️⃣ Feature Queries</h2>
    <div class="feature">
      <div>Si el navegador soporta grid...</div>
      <div>...se muestran en columnas.</div>
    </div>
  </section>

  <section>
    <h2>8️⃣ Container Queries</h2>
    <div class="container">
      <p>Este texto cambia su estilo si el contenedor se reduce, demostrando la adaptabilidad del diseño, igual que los pingüinos en su entorno.</p>
    </div>
  </section>

</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>🐧 Prácticas de Animaciones CSS — Pingüinos Emperador</title>
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(to bottom right, #c3e0ff, #ffd6f5);
      margin: 0;
      padding: 0;
      color: #333;
    }

    header {
      background-color: #6ea8fe;
      color: white;
      text-align: center;
      padding: 20px;
      font-size: 2rem;
      font-weight: bold;
    }

    section {
      background-color: #fff;
      margin: 30px auto;
      padding: 25px;
      border-radius: 20px;
      box-shadow: 0 0 15px rgba(0, 0, 0, 0.1);
      max-width: 1000px;
    }

    h2 {
      color: #ff66b2;
      font-size: 1.8rem;
      border-bottom: 3px solid #6ea8fe;
      padding-bottom: 8px;
      text-align: center;
    }

    p {
      text-align: justify;
      line-height: 1.6;
    }

    /* =======================
       1. TRANSICIONES (REPASO)
    ======================== */
    .caja-transicion {
      width: 150px;
      height: 150px;
      background-color: #99ccff;
      border-radius: 15px;
      margin: 20px auto;
      transition: all 0.5s ease;
    }

    .caja-transicion:hover {
      background-color: #ff99cc;
      transform: rotate(15deg) scale(1.1);
    }

    /* =======================
       2. ANIMACIONES
    ======================== */
    @keyframes moverPingüino {
      0% { transform: translateX(0); }
      50% { transform: translateX(200px); }
      100% { transform: translateX(0); }
    }

    .animacion {
      width: 100px;
      height: 100px;
      background-color: #ffbdf0;
      border-radius: 50%;
      margin: 20px auto;
      animation: moverPingüino 3s infinite ease-in-out;
    }

    /* =======================
       3. BOTONES ANIMADOS Y TYPEWRITER
    ======================== */
    .boton-animado {
      display: block;
      margin: 20px auto;
      padding: 12px 30px;
      font-size: 1.2rem;
      color: white;
      background-color: #6ea8fe;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    .boton-animado:hover {
      background-color: #ff66b2;
    }

    .typewriter {
      overflow: hidden;
      border-right: .15em solid #6ea8fe;
      white-space: nowrap;
      animation: typing 3s steps(40, end), blink .75s step-end infinite;
      width: 0;
      margin: 20px auto;
      font-size: 1.2rem;
      text-align: center;
      color: #333;
    }

    @keyframes typing {
      from { width: 0 }
      to { width: 100% }
    }

    @keyframes blink {
      50% { border-color: transparent }
    }

    /* =======================
       4. ANIMACIONES BASADAS EN SCROLL
    ======================== */
    .scroll {
      opacity: 0;
      transform: translateY(50px);
      transition: all 1s ease-out;
    }

    .scroll.visible {
      opacity: 1;
      transform: translateY(0);
    }

    /* =======================
       5. RANGO DE ANIMACIONES
    ======================== */
    .rango {
      width: 100px;
      height: 100px;
      background: #a4d4ff;
      border-radius: 10px;
      margin: 20px auto;
      animation: cambioColor 4s infinite alternate;
    }

    @keyframes cambioColor {
      0% { background: #a4d4ff; }
      50% { background: #ffbdf0; transform: scale(1.2); }
      100% { background: #6ea8fe; transform: scale(1); }
    }

    /* =======================
       6. INTEGRANDO ANIMACIONES EN UNA WEB
    ======================== */
    .tarjeta {
      background: #f0f8ff;
      padding: 20px;
      border-radius: 20px;
      text-align: center;
      transition: transform 0.4s ease, box-shadow 0.4s ease;
    }

    .tarjeta:hover {
      transform: translateY(-10px);
      box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
    }

    /* =======================
       7. ANIMACIONES: CUMPLIENDO LA PROMESA
    ======================== */
    .corazon {
      position: relative;
      width: 100px;
      height: 90px;
      margin: 30px auto;
      animation: latir 1s infinite;
    }

    .corazon::before,
    .corazon::after {
      content: "";
      position: absolute;
      width: 100px;
      height: 90px;
      background: #ff66b2;
      border-radius: 50%;
      top: 0;
      left: 0;
    }

    .corazon::after {
      left: 50px;
    }

    .corazon {
      transform: rotate(-45deg);
    }

    @keyframes latir {
      0%, 100% { transform: rotate(-45deg) scale(1); }
      50% { transform: rotate(-45deg) scale(1.2); }
    }
  </style>
</head>
<body>

<header>🐧 Prácticas de ANIMACIONES CSS — Pingüinos Emperador</header>

<section>
  <h2>1. Transiciones (Repaso)</h2>
  <div class="caja-transicion"></div>
  <p>Los pingüinos juveniles aprenden gradualmente, como una transición suave entre la tierra y el agua.</p>
</section>

<section>
  <h2>2. Animaciones</h2>
  <div class="animacion"></div>
  <p>Así como los pingüinos se mueven de un lado a otro bajo el hielo, esta animación repite su recorrido.</p>
</section>

<section>
  <h2>3. Botones Animados y Efecto Typewriter</h2>
  <button class="boton-animado">Haz clic aquí 🐧</button>
  <div class="typewriter">Los pingüinos aprenden a nadar por sí mismos...</div>
</section>

<section>
  <h2>4. Animaciones Basadas en Scroll</h2>
  <div class="scroll" id="scrollAnim">
    <p>Cuando los pingüinos se adentran en el océano, comienzan un nuevo viaje lleno de movimiento.</p>
  </div>
</section>

<section>
  <h2>5. Rango de Animaciones</h2>
  <div class="rango"></div>
  <p>El color y tamaño cambian como el ambiente marino donde los pingüinos se adaptan al clima.</p>
</section>

<section>
  <h2>6. Integrando Animaciones en una Web</h2>
  <div class="tarjeta">
    <h3>La Vida del Pingüino</h3>
    <p>Los jóvenes permanecen en el mar durante años antes de regresar a su colonia. Esta tarjeta lo representa con una animación suave al pasar el cursor.</p>
  </div>
</section>

<section>
  <h2>7. Animaciones: Cumpliendo la Promesa</h2>
  <div class="corazon"></div>
  <p>El corazón late como símbolo de la perseverancia y vida de los pingüinos emperador ante el cambio climático.</p>
</section>

<script>
  // Animación al hacer scroll
  const elemento = document.getElementById('scrollAnim');
  window.addEventListener('scroll', () => {
    const posicion = elemento.getBoundingClientRect().top;
    const altura = window.innerHeight;
    if (posicion < altura - 100) {
      elemento.classList.add('visible');
    }
  });
</script>

</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Prácticas — WEB HOSTING | Pingüinos Emperador</title>
  <style>
    /* Estilos generales */
    body {
      font-family: 'Poppins', sans-serif;
      margin: 0;
      background-color: #f2f6ff;
      color: #333;
      line-height: 1.6;
    }

    header {
      text-align: center;
      padding: 40px;
      background: linear-gradient(90deg, #89cff0, #f4b6c2);
      color: white;
      font-size: 2.2em;
      font-weight: bold;
      letter-spacing: 2px;
    }

    section {
      padding: 40px 10%;
      margin: 20px 0;
      border-radius: 20px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    }

    h2 {
      font-size: 1.8em;
      text-align: center;
      color: #004aad;
      background-color: rgba(255, 255, 255, 0.8);
      padding: 15px;
      border-radius: 10px;
      margin-bottom: 20px;
    }

    .azul {
      background-color: #cce6ff;
    }

    .rosa {
      background-color: #ffe0eb;
    }

    p {
      text-align: justify;
      font-size: 1.05em;
    }

    footer {
      text-align: center;
      padding: 30px;
      background-color: #004aad;
      color: white;
      font-size: 1em;
      border-top: 5px solid #f4b6c2;
    }

    .enlace {
      text-align: center;
      margin-top: 15px;
    }

    .enlace a {
      color: #004aad;
      background-color: #fff;
      padding: 10px 20px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: bold;
      transition: 0.3s;
      border: 2px solid #004aad;
    }

    .enlace a:hover {
      background-color: #004aad;
      color: #fff;
    }
  </style>
</head>
<body>

  <header>🌐 Prácticas — WEB HOSTING (Pingüinos Emperador) 🐧</header>

  <!-- SECCIÓN 1 -->
  <section class="azul">
    <h2>1️⃣ Introducción al WEB HOSTING</h2>
    <p>
      El *Web Hosting* o alojamiento web es el servicio que permite almacenar una página en Internet. 
      Imagina que tu sitio es el hogar digital de los **pingüinos emperador**, donde cada archivo, imagen y video 
      vive dentro de un servidor que mantiene la página activa para que otros puedan visitarla desde cualquier parte del mundo.
    </p>
    <p>
      Así como los jóvenes pingüinos aprenden a nadar y explorar nuevas aguas, una web alojada necesita un entorno estable 
      donde pueda crecer, actualizarse y ser descubierta. Los servidores actúan como ese mar inmenso lleno de oportunidades digitales.
    </p>
  </section>

  <!-- SECCIÓN 2 -->
  <section class="rosa">
    <h2>2️⃣ Subir tu WEB a INTERNET</h2>
    <p>
      Para subir tu página web, se necesitan tres elementos principales:
      <strong>dominio</strong> (nombre del sitio), <strong>hosting</strong> (el espacio donde vive tu web) 
      y <strong>archivos</strong> (tu contenido HTML, CSS, imágenes, etc.). 
    </p>
    <p>
      Al igual que los investigadores colocaron rastreadores en los pingüinos para seguir sus movimientos, 
      cuando subes tu web a Internet, estás haciendo visible su “ruta digital”, permitiendo que cualquiera la encuentre 
      usando un navegador. 
    </p>
    <p>
      En el caso de los **pingüinos emperadores juveniles**, aprender a moverse por el océano fue clave para su supervivencia; 
      de forma similar, para un desarrollador web, aprender a publicar un sitio es el paso que marca su independencia digital.
    </p>

    <div class="enlace">
      <a href="https://youtu.be/ELSm-G201Ls?si=WzOM2_6PLuHiht2R" target="_blank">
        🎥 Ver práctica en YouTube
      </a>
    </div>
  </section>

  <footer>
    Proyecto Educativo CSS — Inspirado en los Pingüinos Emperador 🩵💗
  </footer>

</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Prácticas — SECCIÓN AVANZADA | Pingüinos Emperador</title>
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      margin: 0;
      background-color: #f0f6ff;
      color: #333;
      line-height: 1.7;
    }

    header {
      text-align: center;
      background: linear-gradient(90deg, #a1c4fd, #fbc2eb);
      color: white;
      padding: 40px;
      font-size: 2.4em;
      font-weight: bold;
      letter-spacing: 2px;
    }

    section {
      margin: 30px 10%;
      padding: 40px;
      border-radius: 20px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    }

    h2 {
      text-align: center;
      font-size: 1.8em;
      background: rgba(255,255,255,0.8);
      padding: 15px;
      border-radius: 10px;
      color: #004aad;
    }

    .azul {
      background-color: #cce6ff;
    }

    .rosa {
      background-color: #ffe0eb;
    }

    p {
      text-align: justify;
      font-size: 1.05em;
      margin-top: 15px;
    }

    .enlace {
      text-align: center;
      margin-top: 20px;
    }

    .enlace a {
      text-decoration: none;
      color: #004aad;
      background-color: white;
      padding: 10px 20px;
      border: 2px solid #004aad;
      border-radius: 8px;
      font-weight: bold;
      transition: 0.3s;
    }

    .enlace a:hover {
      background-color: #004aad;
      color: white;
    }

    footer {
      text-align: center;
      background-color: #004aad;
      color: white;
      padding: 25px;
      font-size: 1em;
      border-top: 5px solid #fbc2eb;
    }

    /* Ejemplos visuales simples */
    .demo {
      text-align: center;
      margin: 20px 0;
    }

    .demo img {
      width: 200px;
      border-radius: 10px;
      transition: 0.5s;
    }

    .filtro img:hover {
      filter: blur(2px) brightness(1.2);
    }

    .transformar:hover {
      transform: rotate(15deg) scale(1.1);
    }

    .colorMix {
      background: color-mix(in srgb, #89cff0 60%, #f4b6c2);
      padding: 20px;
      border-radius: 10px;
      color: #004aad;
      font-weight: bold;
      text-align: center;
    }

    .scroll-ejemplo {
      overflow-y: scroll;
      max-height: 120px;
      background-color: white;
      padding: 10px;
      border-radius: 10px;
    }

    .scroll-ejemplo::-webkit-scrollbar {
      width: 8px;
    }
    .scroll-ejemplo::-webkit-scrollbar-thumb {
      background: #004aad;
      border-radius: 5px;
    }

    .initial::first-letter {
      initial-letter: 3;
      color: #f46fb0;
      font-weight: bold;
    }

  </style>
</head>
<body>

  <header>💎 Prácticas — SECCIÓN AVANZADA 🐧</header>

  <!-- 1 -->
  <section class="azul">
    <h2>1️⃣ Filter y Backdrop Filter</h2>
    <p>Los filtros permiten aplicar efectos visuales como desenfoque, brillo o contraste. En la investigación sobre los pingüinos, los científicos aplicaron “filtros” digitales para interpretar las señales satelitales y ubicar sus rutas.</p>
    <div class="demo filtro">
      <img src="https://i.pinimg.com/474x/b3/0a/fd/b30afdfc7dded0384102e0c7115398bf.jpg" alt="Pingüino emperador">
    </div>
  </section>

  <!-- 2 -->
  <section class="rosa">
    <h2>2️⃣ Transform</h2>
    <p>La propiedad <b>transform</b> permite rotar, escalar o mover elementos. Así como los pingüinos giran y se adaptan al bucear, los elementos en CSS también pueden transformarse visualmente.</p>
    <div class="demo">
      <img class="transformar" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSmHvbSl2hISkdcOm0j_hEv2Xr9BZDbY-4OnzqSQkxPb-n0iwgfkl3ioqY5TrUHIn1gyf0&usqp=CAU" alt="Polluelo pingüino">
    </div>
  </section>

  <!-- 3 -->
  <section class="azul">
    <h2>3️⃣ Min, Max y Clamp</h2>
    <p>Estas funciones permiten controlar tamaños mínimos, máximos o proporcionales. Por ejemplo, los investigadores usaron límites para determinar la profundidad mínima y máxima del buceo (hasta 264 m).</p>
  </section>

  <!-- 4 -->
  <section class="rosa">
    <h2>4️⃣ Variables (Custom Properties)</h2>
    <p>Las variables en CSS guardan valores reutilizables. Igual que los científicos almacenan datos de comportamiento, nosotros guardamos colores o medidas para mantener coherencia en el diseño.</p>
  </section>

  <!-- 5 -->
  <section class="azul">
    <h2>5️⃣ Función Calc()</h2>
    <p>Permite hacer cálculos dentro del CSS, como combinar porcentajes y píxeles. Tal como los investigadores calcularon la distancia entre colonias y zonas de buceo, nosotros calculamos espacios dinámicos.</p>
  </section>

  <!-- 6 -->
  <section class="rosa">
    <h2>6️⃣ Propiedades del Scroll</h2>
    <p>El desplazamiento (scroll) puede personalizarse para mejorar la experiencia visual. En el estudio, los científicos también “desplazaron” su seguimiento satelital para observar los movimientos de los pingüinos en el tiempo.</p>
    <div class="scroll-ejemplo">
      <p>Los pingüinos juveniles se movieron inicialmente hacia el norte...</p>
      <p>Luego aprendieron a bucear bajo el hielo marino...</p>
      <p>Finalmente regresaron al sur durante el invierno antártico...</p>
    </div>
  </section>

  <!-- 7 -->
  <section class="azul">
    <h2>7️⃣ Initial Letter</h2>
    <p class="initial">En CSS podemos agrandar la primera letra de un texto para dar un efecto editorial elegante. Así resalta la introducción de una historia, como los primeros pasos de los jóvenes pingüinos en el océano.</p>
  </section>

  <!-- 8 -->
  <section class="rosa">
    <h2>8️⃣ Unidades del Viewport (Large, Small y Dynamic)</h2>
    <p>Estas unidades permiten ajustar los tamaños a la vista del usuario, como si los pingüinos ajustaran su dirección dependiendo del tamaño del hielo disponible.</p>
  </section>

  <!-- 9 -->
  <section class="azul">
    <h2>9️⃣ Min-content, Max-content y Fit-content</h2>
    <p>Sirven para definir el espacio que ocupa un elemento según su contenido. En el ecosistema polar, los pingüinos también ajustan su espacio en grupo para conservar calor, como un "fit-content" natural.</p>
  </section>

  <!-- 10 -->
  <section class="rosa">
    <h2>🔟 Función Color Mix()</h2>
    <p>Permite mezclar dos colores en proporciones específicas. Así como el océano y el hielo crean tonalidades únicas en la Antártida, podemos crear combinaciones armónicas de color en CSS.</p>
    <div class="colorMix">Ejemplo de mezcla de colores</div>
  </section>

  <div class="enlace">
    <a href="https://youtu.be/ELSm-G201Ls?si=WzOM2_6PLuHiht2R" target="_blank">
      🎥 Ver video completo en YouTube
    </a>
  </div>

  <footer>
    🌐 Proyecto Educativo — CSS Avanzado con Pingüinos Emperador 🩵💗
  </footer>

</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Proyectos Finales — Sidebar Menu & Chatbox</title>
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      margin: 0;
      background-color: #f0f6ff;
      color: #333;
      line-height: 1.7;
    }

    header {
      text-align: center;
      background: linear-gradient(90deg, #a1c4fd, #fbc2eb);
      color: white;
      padding: 40px;
      font-size: 2.4em;
      font-weight: bold;
      letter-spacing: 2px;
    }

    section {
      margin: 30px 10%;
      padding: 40px;
      border-radius: 20px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    }

    h2 {
      text-align: center;
      font-size: 1.8em;
      background: rgba(255,255,255,0.8);
      padding: 15px;
      border-radius: 10px;
      color: #004aad;
    }

    .azul {
      background-color: #cce6ff;
    }

    .rosa {
      background-color: #ffe0eb;
    }

    p {
      text-align: justify;
      font-size: 1.05em;
      margin-top: 15px;
    }

    footer {
      text-align: center;
      background-color: #004aad;
      color: white;
      padding: 25px;
      font-size: 1em;
      border-top: 5px solid #fbc2eb;
    }

    /* --- PROYECTO 1: SIDEBAR MENU --- */
    .sidebar {
      height: 100%;
      width: 220px;
      position: fixed;
      top: 0;
      left: 0;
      background-color: #89cff0;
      padding-top: 20px;
      border-right: 4px solid #fbc2eb;
    }

    .sidebar a {
      display: block;
      color: #004aad;
      padding: 14px;
      text-decoration: none;
      font-weight: bold;
      transition: 0.3s;
    }

    .sidebar a:hover {
      background-color: #fbc2eb;
      color: white;
      border-radius: 8px;
    }

    .contenido {
      margin-left: 240px;
      padding: 20px;
    }

    /* --- PROYECTO 2: CHATBOX --- */
    .chat-container {
      max-width: 500px;
      margin: 30px auto;
      border-radius: 15px;
      background-color: #ffffff;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      display: flex;
      flex-direction: column;
    }

    .chat-box {
      padding: 20px;
      height: 250px;
      overflow-y: auto;
      background-color: #f9f9ff;
      border-bottom: 2px solid #fbc2eb;
    }

    .mensaje {
      background-color: #cce6ff;
      padding: 10px 15px;
      margin: 10px;
      border-radius: 10px;
      max-width: 70%;
    }

    .usuario {
      align-self: flex-end;
      background-color: #ffe0eb;
    }

    .chat-input {
      display: flex;
      padding: 10px;
      background-color: #f0f6ff;
      border-radius: 0 0 15px 15px;
    }

    .chat-input input {
      flex: 1;
      border: none;
      outline: none;
      padding: 10px;
      border-radius: 10px;
    }

    .chat-input button {
      background-color: #004aad;
      color: white;
      border: none;
      padding: 10px 20px;
      margin-left: 10px;
      border-radius: 10px;
      cursor: pointer;
      transition: 0.3s;
    }

    .chat-input button:hover {
      background-color: #f46fb0;
    }

  </style>
</head>
<body>

  <header>PROYECTOS FINALES — HTML, CSS y JS</header>

  <!-- SECCIÓN 1: SIDEBAR MENU -->
  <section class="azul">
    <h2>Proyecto 1 — Sidebar Menu</h2>

    <div class="sidebar">
      <a href="#">Inicio</a>
      <a href="#">Sobre Nosotros</a>
      <a href="#">Galería</a>
      <a href="#">Contacto</a>
    </div>

    <div class="contenido">
      <h3>Cómo aprenden los pingüinos</h3>
      <p>El equipo liderado por Sara Labrousse, investigadora postdoctoral del WHOI, estudió los comportamientos de los pingüinos emperadores juveniles durante sus primeros meses fuera de la colonia. En este tiempo, los pingüinos aprenden por sí mismos a nadar, bucear y encontrar alimento, sin ayuda de sus padres.</p>
      <p>Los rastreadores instalados en 15 juveniles registraron más de 62,000 inmersiones, demostrando que los jóvenes pingüinos se desplazaron al norte en busca de aguas abiertas y templadas, antes de dirigirse nuevamente hacia el sur bajo el hielo marino.</p>
      <p>Este tipo de investigación es clave para comprender su ciclo de vida y cómo podrían adaptarse al cambio climático en el futuro.</p>
    </div>
  </section>

  <!-- SECCIÓN 2: CHATBOX -->
  <section class="rosa">
    <h2>Proyecto 2 — Chatbox</h2>

    <div class="chat-container">
      <div class="chat-box" id="chatBox">
        <div class="mensaje">Hola 👋 ¿Sabías que los pingüinos emperadores pueden bucear más de 250 metros?</div>
        <div class="mensaje usuario">¡Wow! No tenía idea 🐧 ¿Cómo lo hacen?</div>
        <div class="mensaje">Usan su gran capacidad pulmonar y adaptaciones especiales en su sangre para resistir la presión del agua.</div>
      </div>
      <div class="chat-input">
        <input type="text" id="mensajeInput" placeholder="Escribe tu mensaje..." />
        <button onclick="enviarMensaje()">Enviar</button>
      </div>
    </div>

    <script>
      function enviarMensaje() {
        const input = document.getElementById('mensajeInput');
        const chatBox = document.getElementById('chatBox');
        const texto = input.value.trim();
        if (texto !== "") {
          const nuevoMsg = document.createElement('div');
          nuevoMsg.classList.add('mensaje', 'usuario');
          nuevoMsg.textContent = texto;
          chatBox.appendChild(nuevoMsg);
          chatBox.scrollTop = chatBox.scrollHeight;
          input.value = "";
        }
      }
    </script>

    <p>Los pingüinos juveniles también interactúan de forma social cuando bucean y se agrupan para aprender a cazar y orientarse bajo el hielo marino. Este comportamiento cooperativo puede mejorar sus posibilidades de supervivencia durante los primeros años de vida.</p>
  </section>

  <footer>Práctica Final creada con HTML + CSS + JS — Inspirada en el video del Sidebar & Chatbox (YouTube)</footer>

</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Proyectos Finales — Flip Card & One Page View</title>
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      margin: 0;
      background-color: #f0f6ff;
      color: #333;
      line-height: 1.7;
    }

    header {
      text-align: center;
      background: linear-gradient(90deg, #a1c4fd, #fbc2eb);
      color: white;
      padding: 40px;
      font-size: 2.4em;
      font-weight: bold;
      letter-spacing: 2px;
    }

    section {
      margin: 30px 10%;
      padding: 40px;
      border-radius: 20px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    }

    h2 {
      text-align: center;
      font-size: 1.8em;
      background: rgba(255,255,255,0.8);
      padding: 15px;
      border-radius: 10px;
      color: #004aad;
    }

    .azul {
      background-color: #cce6ff;
    }

    .rosa {
      background-color: #ffe0eb;
    }

    p {
      text-align: justify;
      font-size: 1.05em;
      margin-top: 15px;
    }

    footer {
      text-align: center;
      background-color: #004aad;
      color: white;
      padding: 25px;
      font-size: 1em;
      border-top: 5px solid #fbc2eb;
    }

    /* --- FLIP CARD --- */
    .flip-container {
      perspective: 1000px;
      display: flex;
      justify-content: center;
      margin-top: 30px;
    }

    .flip-card {
      width: 250px;
      height: 300px;
      position: relative;
      transform-style: preserve-3d;
      transition: transform 0.8s;
    }

    .flip-card:hover {
      transform: rotateY(180deg);
    }

    .flip-card-front, .flip-card-back {
      position: absolute;
      width: 100%;
      height: 100%;
      backface-visibility: hidden;
      border-radius: 15px;
      overflow: hidden;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    }

    .flip-card-front {
      background-color: #a1c4fd;
      color: white;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      font-size: 1.3em;
      padding: 20px;
    }

    .flip-card-back {
      background-color: #fbc2eb;
      color: #333;
      transform: rotateY(180deg);
      padding: 20px;
      display: flex;
      flex-direction: column;
      justify-content: center;
      text-align: center;
    }

    /* --- ONE PAGE VIEW --- */
    .contenedor-onepage {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 25px;
      margin-top: 30px;
    }

    .tarjeta {
      background: white;
      border-radius: 15px;
      padding: 20px;
      text-align: center;
      transition: transform 0.3s, box-shadow 0.3s;
    }

    .tarjeta:hover {
      transform: translateY(-10px);
      box-shadow: 0 8px 16px rgba(0,0,0,0.2);
    }

    .tarjeta img {
      width: 100%;
      height: 180px;
      object-fit: cover;
      border-radius: 10px;
      margin-bottom: 10px;
    }

    .tarjeta h3 {
      color: #004aad;
      font-size: 1.2em;
    }

    .tarjeta p {
      font-size: 0.95em;
    }
  </style>
</head>
<body>

  <header>Proyectos Finales — Flip Card & One Page View</header>

  <!-- SECCIÓN 1: FLIP CARD -->
  <section class="azul">
    <h2>Práctica 3 — Flip Card</h2>
    <p>
      Los pingüinos emperadores juveniles viven un proceso de aprendizaje crucial al abandonar su colonia natal. 
      Al principio, son torpes e inseguros, pero con el tiempo se convierten en expertos buceadores capaces de alcanzar 
      profundidades de hasta 264 metros. Este aprendizaje ocurre sin la guía de los padres, mostrando un instinto natural 
      de supervivencia sorprendente.
    </p>

    <div class="flip-container">
      <div class="flip-card">
        <div class="flip-card-front">
          🐧
          <p>Aprendiendo a Nadar</p>
        </div>
        <div class="flip-card-back">
          <p>Los pingüinos juveniles practican buceando bajo el hielo marino durante el invierno, ganando experiencia y fuerza para sobrevivir en condiciones extremas.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- SECCIÓN 2: ONE PAGE VIEW -->
  <section class="rosa">
    <h2>Práctica 4 — One Page View</h2>
    <p>
      El estudio de Sara Labrousse y su equipo ha revelado cómo los jóvenes pingüinos emperadores se adaptan 
      a las duras condiciones antárticas. Se desplazaron hacia el norte para aprender a nadar y luego regresaron 
      al sur, buceando bajo el hielo durante el invierno. Estas observaciones son esenciales para comprender su 
      supervivencia frente al cambio climático.
    </p>

    <div class="contenedor-onepage">
      <div class="tarjeta">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQgxCWuLwuE3Tfh5FR0ptg0DgItYIz5qVV1zA&s" alt="Pingüino Emperador">
        <h3>La vida de Emperador</h3>
        <p>Los machos incuban los huevos mientras las hembras cazan. Su ciclo depende del hielo marino, lo que los hace vulnerables al cambio climático.</p>
      </div>
      <div class="tarjeta">
        <img src="https://www.vistaalmar.es/images/ampliadas387/pinguino-emperador-buceando.jpg" alt="Pingüino Juvenil">
        <h3>Buceando entre dos aguas</h3>
        <p>Los jóvenes bucean en la termoclina, donde se concentran sus presas, aprendiendo a cazar de forma independiente.</p>
      </div>
      <div class="tarjeta">
        <img src="https://storage.googleapis.com/oceanwide_web/media-dynamic/cache/list_photo/v2-gallery_media/media67b70cd98fe9b844894570.jpg" alt="Colonia de pingüinos">
        <h3>Adaptación al clima</h3>
        <p>Comprender cómo responden los pingüinos a los cambios del entorno es clave para proteger su especie en el futuro.</p>
      </div>
    </div>
  </section>

  <footer>
    © 2025 — Prácticas finales HTML & CSS | Inspirado en video tutorial de diseño web
  </footer>

</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Proyecto 5 — Menú Acordeón</title>
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      margin: 0;
      background-color: #f0f6ff;
      color: #333;
      line-height: 1.7;
    }

    header {
      text-align: center;
      background: linear-gradient(90deg, #a1c4fd, #fbc2eb);
      color: white;
      padding: 40px;
      font-size: 2.4em;
      font-weight: bold;
      letter-spacing: 2px;
    }

    section {
      margin: 30px 10%;
      padding: 40px;
      border-radius: 20px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    }

    h2 {
      text-align: center;
      font-size: 1.8em;
      background: rgba(255,255,255,0.8);
      padding: 15px;
      border-radius: 10px;
      color: #004aad;
    }

    .azul {
      background-color: #cce6ff;
    }

    p {
      text-align: justify;
      font-size: 1.05em;
      margin-top: 15px;
    }

    footer {
      text-align: center;
      background-color: #004aad;
      color: white;
      padding: 25px;
      font-size: 1em;
      border-top: 5px solid #fbc2eb;
    }

    /* --- ESTILOS DEL ACORDEÓN --- */
    .acordeon {
      width: 100%;
      max-width: 700px;
      margin: 0 auto;
    }

    .acordeon-item {
      background-color: white;
      margin-bottom: 15px;
      border-radius: 10px;
      box-shadow: 0 3px 8px rgba(0,0,0,0.1);
      overflow: hidden;
      transition: 0.3s;
    }

    .acordeon-titulo {
      background: linear-gradient(90deg, #a1c4fd, #fbc2eb);
      color: #004aad;
      cursor: pointer;
      padding: 15px 20px;
      font-size: 1.2em;
      font-weight: bold;
      display: flex;
      justify-content: space-between;
      align-items: center;
      border: none;
      width: 100%;
      text-align: left;
      transition: 0.3s;
    }

    .acordeon-titulo:hover {
      background: linear-gradient(90deg, #89cff0, #f4b6c2);
    }

    .acordeon-titulo::after {
      content: "+";
      font-size: 1.5em;
      transition: 0.3s;
    }

    .acordeon-item.activo .acordeon-titulo::after {
      content: "−";
    }

    .acordeon-contenido {
      max-height: 0;
      overflow: hidden;
      transition: max-height 0.4s ease, padding 0.3s;
      background-color: #fdfdff;
      padding: 0 20px;
    }

    .acordeon-item.activo .acordeon-contenido {
      max-height: 500px;
      padding: 15px 20px;
    }
  </style>
</head>
<body>

  <header>Proyecto 5 — Menú Acordeón</header>

  <section class="azul">
    <h2>Práctica 5 — Menú Acordeón</h2>
    <p>
      En esta práctica se presenta un menú acordeón interactivo con información sobre el aprendizaje y la vida
      de los pingüinos emperadores. Este diseño permite organizar contenido de manera visual y dinámica, 
      inspirado en los proyectos del video de referencia.
    </p>

    <div class="acordeon">
      <!-- ITEM 1 -->
      <div class="acordeon-item">
        <button class="acordeon-titulo">1. Cómo aprenden los pingüinos</button>
        <div class="acordeon-contenido">
          <p>
            El equipo liderado por Sara Labrousse, investigadora postdoctoral del WHOI, estudió el comportamiento 
            de los pingüinos emperadores juveniles en sus primeros meses tras abandonar la colonia. 
            Sin guía parental, aprenden a nadar, bucear y buscar alimento, lo cual es esencial para su supervivencia.
          </p>
        </div>
      </div>

      <!-- ITEM 2 -->
      <div class="acordeon-item">
        <button class="acordeon-titulo">2. Buceando entre dos aguas</button>
        <div class="acordeon-contenido">
          <p>
            Los datos satelitales mostraron más de 62,000 inmersiones. Al principio se desplazaron hacia el norte 
            buscando aguas abiertas; luego, ya experimentados, regresaron al sur y bucearon bajo el hielo marino. 
            La inmersión más profunda registrada fue de 264 metros.
          </p>
        </div>
      </div>

      <!-- ITEM 3 -->
      <div class="acordeon-item">
        <button class="acordeon-titulo">3. Relación con la termoclina</button>
        <div class="acordeon-contenido">
          <p>
            Los científicos descubrieron que la profundidad del buceo está relacionada con la termoclina, 
            la capa donde se mezclan aguas cálidas y frías. En esa zona se concentran sus presas como el krill, 
            lo que les permite perfeccionar sus habilidades de caza.
          </p>
        </div>
      </div>

      <!-- ITEM 4 -->
      <div class="acordeon-item">
        <button class="acordeon-titulo">4. La vida de emperador</button>
        <div class="acordeon-contenido">
          <p>
            Los pingüinos emperadores son los más grandes de su especie y dependen profundamente del hielo marino. 
            Los machos incuban los huevos mientras las hembras cazan. Un cambio en el hielo marino afecta su 
            alimentación y supervivencia, volviéndolos vulnerables al cambio climático.
          </p>
        </div>
      </div>

      <!-- ITEM 5 -->
      <div class="acordeon-item">
        <button class="acordeon-titulo">5. Adaptación y futuro</button>
        <div class="acordeon-contenido">
          <p>
            Los jóvenes permanecen entre cinco y seis años en el mar antes de regresar para reproducirse. 
            Comprender cómo responden al cambio climático es clave para predecir la supervivencia de la especie 
            y las posibles variaciones en su población futura.
          </p>
        </div>
      </div>
    </div>
  </section>

  <footer>
    © 2025 — Proyecto Final HTML & CSS | Menú Acordeón inspirado en video tutorial
  </footer>

  <script>
    // SCRIPT PARA EL ACORDEÓN
    const items = document.querySelectorAll('.acordeon-item');

    items.forEach(item => {
      const titulo = item.querySelector('.acordeon-titulo');
      titulo.addEventListener('click', () => {
        const activo = item.classList.contains('activo');
        items.forEach(i => i.classList.remove('activo'));
        if (!activo) item.classList.add('activo');
      });
    });
  </script>

</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Proyectos Finales — Cómo Seguir Aprendiendo</title>
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      margin: 0;
      background-color: #f0f6ff;
      color: #333;
      line-height: 1.7;
    }

    header {
      text-align: center;
      background: linear-gradient(90deg, #a1c4fd, #fbc2eb);
      color: white;
      padding: 40px;
      font-size: 2.4em;
      font-weight: bold;
      letter-spacing: 2px;
    }

    section {
      margin: 30px 10%;
      padding: 40px;
      border-radius: 20px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    }

    h2 {
      text-align: center;
      font-size: 1.8em;
      background: rgba(255,255,255,0.8);
      padding: 15px;
      border-radius: 10px;
      color: #004aad;
    }

    .azul {
      background-color: #cce6ff;
    }

    .rosa {
      background-color: #ffe0eb;
    }

    p {
      text-align: justify;
      font-size: 1.05em;
      margin-top: 15px;
    }

    footer {
      text-align: center;
      background-color: #004aad;
      color: white;
      padding: 25px;
      font-size: 1em;
      border-top: 5px solid #fbc2eb;
    }

    /* ==== SECCIÓN 1: CÓMO SEGUIR APRENDIENDO ==== */
    .card-container {
      display: flex;
      justify-content: space-evenly;
      flex-wrap: wrap;
      margin-top: 30px;
      gap: 20px;
    }

    .card {
      background-color: white;
      border-radius: 15px;
      width: 250px;
      text-align: center;
      padding: 20px;
      transition: 0.4s;
      box-shadow: 0 4px 8px rgba(0,0,0,0.15);
    }

    .card:hover {
      transform: translateY(-10px) scale(1.05);
      box-shadow: 0 8px 20px rgba(0,0,0,0.2);
    }

    .card img {
      width: 100%;
      height: 160px;
      object-fit: cover;
      border-radius: 10px;
      margin-bottom: 10px;
    }

    .card h3 {
      color: #004aad;
    }

    /* ==== SECCIÓN 2: ANIMACIÓN DE APRENDIZAJE ==== */
    .animacion {
      text-align: center;
      margin-top: 40px;
    }

    .ping {
      width: 120px;
      animation: flotar 3s ease-in-out infinite;
    }

    @keyframes flotar {
      0% { transform: translateY(0); }
      50% { transform: translateY(-15px); }
      100% { transform: translateY(0); }
    }

    .mensaje {
      background: white;
      padding: 15px;
      border-radius: 10px;
      margin-top: 15px;
      display: inline-block;
      color: #004aad;
      font-weight: bold;
    }

    /* BOTONES ENLACE */
    .enlace {
      text-align: center;
      margin-top: 25px;
    }

    .enlace a {
      text-decoration: none;
      color: #004aad;
      background-color: white;
      padding: 10px 20px;
      border: 2px solid #004aad;
      border-radius: 8px;
      font-weight: bold;
      transition: 0.3s;
    }

    .enlace a:hover {
      background-color: #004aad;
      color: white;
    }
  </style>
</head>
<body>

  <header>Proyectos Finales — Cómo Seguir Aprendiendo</header>

  <!-- SECCIÓN 1 -->
  <section class="azul">
    <h2>Práctica 5 — Cómo Seguir Aprendiendo</h2>
    <p>
      Los pingüinos emperadores juveniles aprenden por sí mismos, sin la guía de sus padres. 
      Cuando abandonan la colonia, comienzan un proceso de autodescubrimiento que les permite 
      dominar el nado y la caza bajo condiciones extremas. 
      Este instinto de aprendizaje natural refleja cómo el conocimiento puede adquirirse con 
      exploración, práctica y persistencia.
    </p>

    <div class="card-container">
      <div class="card">
        <img src="https://www.laizquierdadiario.com/IMG/arton128757.jpg?1556320841" alt="Pingüino adulto">
        <h3>Aprender Observando</h3>
        <p>Los jóvenes observan el entorno, descubriendo qué lugares son seguros y dónde pueden encontrar alimento.</p>
      </div>

      <div class="card">
        <img src="https://images.ecestaticos.com/YRue270E1dip5CGLZBIa0wzfaZI=/79x0:718x478/1200x900/filters:fill(white):format(jpg)/f.elconfidencial.com%2Foriginal%2Fcd8%2Ff98%2F665%2Fcd8f986650487b5c2da5432ebe34b99e.jpg" alt="Pingüino juvenil">
        <h3>Aprender Practicando</h3>
        <p>Con cada inmersión ganan confianza. No hay enseñanza directa, solo experiencia y adaptación constante.</p>
      </div>

      <div class="card">
        <img src="https://media.istockphoto.com/id/523883736/es/foto/emperador-penguins-con-chick.jpg?s=612x612&w=0&k=20&c=S69ULlIcsn6tKbTCjIfmLkoTMRMqCF0tSCvBsWOlkrs=" alt="Colonia de pingüinos">
        <h3>Aprender Juntos</h3>
        <p>Las colonias son espacios de comunidad y aprendizaje compartido, reflejando el valor de la colaboración.</p>
      </div>
    </div>

    <div class="enlace">
      <a href="https://youtu.be/ELSm-G201Ls" target="_blank">Ver Video Base</a>
    </div>
  </section>

  <!-- SECCIÓN 2 -->
  <section class="rosa">
    <h2>Práctica 6 — Aprendizaje Continuo</h2>
    <p>
      Así como los pingüinos aprenden de su entorno, nosotros también podemos seguir aprendiendo 
      cada día. Observar, practicar y compartir conocimiento fortalece nuestras habilidades. 
      La curiosidad, la constancia y la paciencia son el motor del crecimiento personal.
    </p>

    <div class="animacion">
      <img class="ping" src="https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcShIH6q7Lw8n78lcqvSmIzd6YZVxuu9hTuKxOQfF1tusu3Z9MikrDv5Uq9axnJQBobl5N1SmXtuMJp7us2vE1CIKs7ApydrbGLRPDdjAw" alt="Pingüino animado">
      <div class="mensaje">¡Sigue aprendiendo y avanzando paso a paso!</div>
    </div>

    <div class="enlace">
      <a href="#top">Volver arriba</a>
    </div>
  </section>

  <footer>
    © 2025 — Prácticas finales HTML & CSS | Basado en el video "Cómo seguir aprendiendo"
  </footer>

</body>
</html>
