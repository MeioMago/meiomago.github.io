<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Para Manu 💖</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #fff0f5;
      margin: 0;
      padding: 0;
    }
    header {
      background-color: #ff69b4;
      color: white;
      text-align: center;
      padding: 1em;
    }
    nav {
      display: flex;
      justify-content: center;
      background-color: #ffc0cb;
    }
    nav button {
      background: none;
      border: none;
      padding: 1em;
      cursor: pointer;
      font-size: 1em;
    }
    nav button:hover {
      background-color: #ffb6c1;
    }
    section {
      display: none;
      padding: 2em;
    }
    section.active {
      display: block;
    }
  </style>
</head>
<body>
  <header>
    <h1>Bem-vinda, Manu 💕</h1>
    <p>Esse site é só pra você :)</p>
  </header>

  <nav>
    <button onclick="showTab('galeria')">Galeria de Fotos</button>
    <button onclick="showTab('textos')">Textos Diários</button>
    <button onclick="showTab('motivos')">Motivos para eu te amar</button>
    <button onclick="showTab('musica')">Nossa Música</button>
  </nav>

  <section id="galeria" class="active">
    <h2>Galeria de Fotos</h2>
    <p>Aqui ficarão nossas fotos mais especiais. 💑</p>
    <!-- Exemplo: <img src="foto1.jpg" alt="Foto nossa" width="200"> -->
  </section>

  <section id="textos">
    <h2>Textos Diários</h2>
    <p>Aqui vou deixar mensagens pra você sempre que der. ✍️</p>
    <p><strong>01/01/2025:</strong> Hoje pensei em você o dia todo, como sempre. Eu te amo! 💖</p>
  </section>

  <section id="motivos">
    <h2>Motivos para te Amar</h2>
    <ol>
      <li>Seu sorriso</li>
      <li>Sua atenção comigo</li>
      <li>O jeito que você me apoia</li>
      <li>Sua risada/li>
      <li>Seu jeitinho</li>
      <li>O jeito que vc mexe com meu coração</li>
      <li>Seu cabelo</li>
      <li>Seu corpo</li>
      <li>Seu cheiro</li>
      <li>O seu jeiro único de fazer tudo certinho</li>
      <li>Seu amor por animais</li>
      <!-- Complete os 10 motivos depois -->
    </ol>
  </section>

  <section id="musica">
    <h2>Nossa Música</h2>
    <p>Essa música me lembra muito você:</p>
    <iframe width="300" height="170" src="https://www.youtube.com/watch?v=nyuo9-OjNNg" frameborder="0" allowfullscreen></iframe>
  </section>

  <script>
    function showTab(tabId) {
      const sections = document.querySelectorAll('section');
      sections.forEach(section => {
        section.classList.remove('active');
      });
      document.getElementById(tabId).classList.add('active');
    }
  </script>
</body>
</html>
