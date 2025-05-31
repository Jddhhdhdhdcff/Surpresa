<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <title>Para Aninha 💖</title>
  <style>
    html, body {
      margin: 0;
      padding: 0;
      height: 100%;
      background: linear-gradient(120deg, #ff69b4 0%, #000 50%, #00bfff 100%);
      background-size: 400% 400%;
      color: white;
      font-family: 'Arial', sans-serif;
      text-align: center;
      overflow-y: auto; /* permite scroll vertical */
      animation: none;
    }

    body {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: flex-start; /* alinha do topo, não centraliza verticalmente */
      min-height: 100vh; /* garante que tenha no mínimo a altura da tela */
      padding: 20px 10px; /* um pequeno espaçamento nas laterais e topo */
    }

    h1 {
      margin-bottom: 30px;
      font-size: 28px;
    }

    button {
      background-color: #ffffff;
      color: #000;
      border: none;
      padding: 15px 30px;
      font-size: 18px;
      border-radius: 8px;
      cursor: pointer;
      transition: all 0.3s;
      margin-bottom: 30px;
    }
    button:hover {
      background-color: #ff69b4;
      color: white;
    }
    #mensagem {
      display: none;
      margin-top: 30px;
      white-space: pre-line;
      max-width: 600px;
    }
    .frase-principal {
      font-size: 48px;
      font-weight: bold;
      color: #fff;
    }
    .titulo-grande {
      font-size: 32px;
      margin-bottom: 10px;
    }
    .mensagem-extra {
      font-size: 18px;
      margin-top: 10px;
      font-style: italic;
      color: #ffc0cb;
    }
    @keyframes ondas {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }
  </style>
</head>
<body>

  <h1 id="titulo">Tem algo especial aqui... 👀</h1>
  <button id="revelar" onclick="mostrarMensagem()">Revelar Mensagem</button>

  <div id="mensagem">
    <p class="frase-principal">para a menina mais bonita do mundo 💖</p>
    <p class="titulo-grande">FELIZ ANIVERSÁRIO! 🥳🎁</p>
    <p class="mensagem-extra">(eu sei que não te dei tantas coisas mas eu dei de coração, espero que goste aninha &lt;3)</p>
    <p style="margin-top: 20px;">Você é a garota mais linda que eu já vi,
mais radiante que o brilho do sol sobre um campo de lírios,
teu sorriso ilumina meus dias,
e teu olhar doce me conquista mais a cada instante.

São tantas coisas que eu amo em você
que palavras não bastariam para contar,
cada detalhe seu é uma poesia
que meu coração insiste em recitar.

Espero que dê tudo certo entre nós,
e o meu maior presente vai ser te ver,
de segunda a sexta,
incomodando você todo dia :3

Feliz aniversário aninha,
amo tu 💖 <3</p>
  </div>

  <audio id="musica" src="https://files.catbox.moe/d4skbx.mp3"></audio>

  <script>
    function mostrarMensagem() {
      document.getElementById("mensagem").style.display = "block";
      document.getElementById("revelar").style.display = "none";
      document.getElementById("titulo").style.display = "none";

      const musica = document.getElementById("musica");
      musica.currentTime = 65;
      musica.play();

      // Ativa o efeito de ondas no fundo
      document.body.style.animation = "ondas 12s ease-in-out infinite";
    }
  </script>

</body>
</html>
