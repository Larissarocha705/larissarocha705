<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>README.md - Perfil Dev</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', 'Poppins', 'Arial', sans-serif;
            background: linear-gradient(135deg, #ffe6f0 0%, #ffd9e8 100%);
            min-height: 100vh;
            padding: 40px 20px;
        }

        /* Container estilo pergaminho de anime */
        .container {
            max-width: 900px;
            margin: 0 auto;
            background: rgba(255, 245, 250, 0.95);
            border-radius: 30px;
            box-shadow: 0 20px 40px rgba(255, 105, 180, 0.2), 0 0 0 2px #ffb6c1, 0 0 0 6px #ffe0e7;
            overflow: hidden;
            backdrop-filter: blur(2px);
            transition: transform 0.3s ease;
        }

        .container:hover {
            transform: translateY(-5px);
        }

        /* Header com estilo anime */
        .header {
            background: linear-gradient(120deg, #ffb7c5, #ff9eb0);
            padding: 40px 30px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .header::before {
            content: "🌸 ✨ 🎀";
            position: absolute;
            font-size: 80px;
            opacity: 0.1;
            bottom: -20px;
            right: -20px;
            transform: rotate(-15deg);
            pointer-events: none;
        }

        .header::after {
            content: "⚡ 🍜 💻";
            position: absolute;
            font-size: 70px;
            opacity: 0.1;
            top: -20px;
            left: -20px;
            transform: rotate(10deg);
            pointer-events: none;
        }

        .avatar {
            width: 120px;
            height: 120px;
            background: linear-gradient(135deg, #ffd1dc, #ffb3c6);
            border-radius: 50%;
            margin: 0 auto 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 60px;
            border: 4px solid white;
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }

        .avatar:hover {
            transform: scale(1.05) rotate(5deg);
        }

        h1 {
            color: #fff;
            font-size: 2.5em;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
            letter-spacing: 2px;
            font-weight: bold;
        }

        .subtitle {
            color: #fff;
            font-size: 1.1em;
            margin-top: 10px;
            opacity: 0.95;
            font-style: italic;
        }

        /* Conteúdo principal */
        .content {
            padding: 40px 35px;
        }

        /* Seções estilo diálogo de anime */
        .section {
            margin-bottom: 35px;
            background: white;
            border-radius: 20px;
            padding: 25px;
            box-shadow: 0 5px 15px rgba(255, 105, 180, 0.1);
            transition: all 0.3s;
            border-left: 5px solid #ffb7c5;
        }

        .section:hover {
            transform: translateX(8px);
            box-shadow: 0 8px 20px rgba(255, 105, 180, 0.15);
        }

        .section-title {
            font-size: 1.8em;
            color: #ff6b8a;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 12px;
            border-bottom: 2px dashed #ffcdd9;
            padding-bottom: 10px;
        }

        .section-title span {
            font-size: 1.2em;
        }

        /* Cards de linguagens */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
            gap: 15px;
            margin-top: 20px;
        }

        .skill-card {
            background: linear-gradient(135deg, #fff5f8, #ffeef3);
            border-radius: 15px;
            padding: 15px;
            text-align: center;
            transition: all 0.3s;
            border: 1px solid #ffcdd9;
            cursor: default;
        }

        .skill-card:hover {
            transform: translateY(-5px) scale(1.02);
            box-shadow: 0 10px 20px rgba(255, 105, 180, 0.2);
            border-color: #ff9eb0;
        }

        .skill-icon {
            font-size: 2.5em;
            margin-bottom: 8px;
        }

        .skill-name {
            font-weight: bold;
            color: #ff6b8a;
            font-size: 1.1em;
        }

        /* Frase estilo anime */
        .quote {
            text-align: center;
            margin-top: 30px;
            padding: 20px;
            background: #fff0f5;
            border-radius: 50px;
            font-style: italic;
            color: #ff6b8a;
            font-weight: 500;
            border: 1px solid #ffcdd9;
        }

        .quote-text {
            font-size: 1.1em;
        }

        .quote-author {
            margin-top: 8px;
            font-size: 0.9em;
            opacity: 0.8;
        }

        /* Badges */
        .badge-container {
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
            margin-top: 20px;
            justify-content: center;
        }

        .badge {
            background: #ffb7c5;
            color: white;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.85em;
            font-weight: bold;
        }

        footer {
            background: #ffd9e4;
            padding: 20px;
            text-align: center;
            color: #ff6b8a;
            font-size: 0.9em;
        }

        @media (max-width: 600px) {
            .content {
                padding: 25px 20px;
            }
            h1 {
                font-size: 1.8em;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="avatar">
                👩‍💻✨
            </div>
            <h1>🌸 Yuna Kimura 🌸</h1>
            <div class="subtitle">
                「 Code is my magic spell • Desenvolvedora em evolução 」
            </div>
        </div>

        <div class="content">
            <!-- Sobre Mim -->
            <div class="section">
                <div class="section-title">
                    <span>📖</span> Sobre Mim
                </div>
                <p style="line-height: 1.6; color: #555;">
                    Olá! Eu sou a <strong>Yuna</strong>, uma desenvolvedora apaixonada por tecnologia, animes e café ☕✨. 
                    Assim como uma protagonista de shonen, estou sempre em busca de evoluir minhas habilidades e superar novos desafios. 
                    Acredito que programação é como aprender um novo jutsu: requer prática, dedicação e criatividade! 🍥
                </p>
            </div>

            <!-- Formação Acadêmica -->
            <div class="section">
                <div class="section-title">
                    <span>🎓</span> Formação
                </div>
                <div style="margin-bottom: 15px;">
                    <strong style="color: #ff6b8a;">💻 Desenvolvimento de Sistemas</strong>
                    <p style="color: #666; margin-top: 5px;">Técnico em Desenvolvimento de Sistemas • Em andamento</p>
                </div>
                <div>
                    <strong style="color: #ff6b8a;">🎓 Ciência da Computação</strong>
                    <p style="color: #666; margin-top: 5px;">Graduação • Buscando conhecimento profundo em algoritmos e inovação</p>
                </div>
            </div>

            <!-- Tecnologias / Linguagens -->
            <div class="section">
                <div class="section-title">
                    <span>⚡</span> Meu Arsenal Ninja
                </div>
                <div class="skills-grid">
                    <div class="skill-card">
                        <div class="skill-icon">🟨</div>
                        <div class="skill-name">JavaScript</div>
                        <div style="font-size: 0.8em; color: #888;">ES6+</div>
                    </div>
                    <div class="skill-card">
                        <div class="skill-icon">🐍</div>
                        <div class="skill-name">Python</div>
                        <div style="font-size: 0.8em; color: #888;">Data & Backend</div>
                    </div>
                    <div class="skill-card">
                        <div class="skill-icon">🌐</div>
                        <div class="skill-name">HTML5</div>
                        <div style="font-size: 0.8em; color: #888;">Estrutura</div>
                    </div>
                    <div class="skill-card">
                        <div class="skill-icon">🎨</div>
                        <div class="skill-name">CSS3</div>
                        <div style="font-size: 0.8em; color: #888;">Estilização</div>
                    </div>
                    <div class="skill-card">
                        <div class="skill-icon">⚛️</div>
                        <div class="skill-name">React</div>
                        <div style="font-size: 0.8em; color: #888;">Em estudo</div>
                    </div>
                    <div class="skill-card">
                        <div class="skill-icon">🗄️</div>
                        <div class="skill-name">SQL</div>
                        <div style="font-size: 0.8em; color: #888;">Database</div>
                    </div>
                </div>
            </div>

            <!-- Estatísticas e Badges -->
            <div class="badge-container">
                <span class="badge">✨ 500+ horas de código</span>
                <span class="badge">🎌 Otaku Dev</span>
                <span class="badge">☕ Café-dependente</span>
                <span class="badge">📚 Sempre aprendendo</span>
            </div>

            <!-- Frase Inspiradora Anime -->
            <div class="quote">
                <div class="quote-text">
                    "Assim como Naruto nunca desistiu de se tornar Hokage,<br>
                    eu nunca vou desistir de evoluir como dev. Dattebayo! 💪🍥"
                </div>
                <div class="quote-author">
                    — Yuna, no seu grind diário
                </div>
            </div>

            <!-- Contato / Redes Sociais (exemplo) -->
            <div style="text-align: center; margin-top: 30px;">
                <div style="display: inline-flex; gap: 20px; font-size: 1.8em;">
                    <span style="cursor: pointer;" title="GitHub">🐙</span>
                    <span style="cursor: pointer;" title="LinkedIn">🔗</span>
                    <span style="cursor: pointer;" title="Twitter/X">🐦</span>
                    <span style="cursor: pointer;" title="Discord">🎮</span>
                </div>
                <p style="color: #ff8aa8; margin-top: 15px; font-size: 0.85em;">
                    💌 yuna.kimura@dev.com • Disponível para novos projetos e parcerias
                </p>
            </div>
        </div>

        <footer>
            🌸 "O verdadeiro poder está em nunca parar de codar" 🌸<br>
            © 2024 Yuna Kimura • Feito com 💖 e muito café
        </footer>
    </div>
</body>
</html>

###

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/larissarocha705/larissarocha705/output/pacman-contribution-graph-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/larissarocha705/larissarocha705/output/pacman-contribution-graph.svg">
  <img alt="pacman contribution graph" src="https://raw.githubusercontent.com/larissarocha705/larissarocha705/output/pacman-contribution-graph.svg">
</picture>



<!--
**Larissarocha705/larissarocha705** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.


