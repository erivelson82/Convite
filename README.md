<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aniversário Vingadores Lego 2026</title>
    <!-- Google Fonts & FontAwesome -->
    <link href="https://fonts.googleapis.com/css2?family=Bangers&family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            --primary: #e63946; /* Vermelho Herói */
            --secondary: #ffb703; /* Amarelo Lego */
            --dark: #1d3557; /* Azul Escuro */
            --light: #f1faee;
            --accent: #457b9d;
            --bg-color: #0f172a;
            --card-bg: #1e293b;
            --text-color: #f8fafc;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-color);
            min-height: 100vh;
            display: flex;
            flex-direction: column;
        }

        header {
            background: linear-gradient(135deg, #1d3557, #e63946);
            padding: 2rem 1rem;
            text-align: center;
            border-bottom: 4px solid var(--secondary);
        }

        header h1 {
            font-family: 'Bangers', cursive;
            font-size: 3rem;
            letter-spacing: 2px;
            color: var(--secondary);
            text-shadow: 3px 3px #000;
        }

        header p {
            font-size: 1.1rem;
            margin-top: 0.5rem;
            font-weight: 600;
        }

        /* Navegação */
        nav {
            background: #111827;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 0.5rem;
            padding: 0.8rem;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 4px 6px rgba(0,0,0,0.3);
        }

        nav button {
            background: var(--card-bg);
            border: 2px solid transparent;
            color: var(--text-color);
            padding: 0.5rem 1rem;
            border-radius: 8px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            gap: 0.4rem;
        }

        nav button:hover, nav button.active {
            background: var(--primary);
            border-color: var(--secondary);
            transform: translateY(-2px);
        }

        main {
            flex: 1;
            max-width: 900px;
            width: 100%;
            margin: 2rem auto;
            padding: 0 1rem;
        }

        .page {
            display: none;
            background: var(--card-bg);
            padding: 2rem;
            border-radius: 16px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.5);
            animation: fadeIn 0.4s ease-in-out;
            border: 2px solid rgba(255,183,3,0.2);
        }

        .page.active {
            display: block;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        h2 {
            font-family: 'Bangers', cursive;
            font-size: 2.2rem;
            color: var(--secondary);
            margin-bottom: 1.5rem;
            letter-spacing: 1px;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        /* Countdown */
        .countdown-container {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin: 2rem 0;
            flex-wrap: wrap;
        }

        .countdown-box {
            background: #0f172a;
            border: 2px solid var(--secondary);
            padding: 1rem 1.5rem;
            border-radius: 12px;
            text-align: center;
            min-width: 90px;
        }

        .countdown-box span {
            font-size: 2rem;
            font-weight: 700;
            color: var(--primary);
            display: block;
        }

        .countdown-box label {
            font-size: 0.85rem;
            text-transform: uppercase;
            color: #94a3b8;
        }

        /* Formulários e Inputs */
        .form-group {
            margin-bottom: 1.2rem;
        }

        label {
            display: block;
            margin-bottom: 0.4rem;
            font-weight: 600;
        }

        input, select, textarea {
            width: 100%;
            padding: 0.8rem;
            border-radius: 8px;
            border: 1px solid #475569;
            background: #0f172a;
            color: white;
            font-size: 1rem;
        }

        input:focus, select:focus, textarea:focus {
            outline: none;
            border-color: var(--secondary);
        }

        button.btn-action {
            background: var(--primary);
            color: white;
            border: none;
            padding: 0.8rem 1.5rem;
            border-radius: 8px;
            font-size: 1rem;
            font-weight: bold;
            cursor: pointer;
            transition: background 0.3s;
            width: 100%;
            margin-top: 1rem;
        }

        button.btn-action:hover {
            background: #c1121f;
        }

        /* Cards e Listas */
        .grid-menu {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-top: 1rem;
        }

        .menu-card {
            background: #0f172a;
            padding: 1.5rem;
            border-radius: 12px;
            border-left: 5px solid var(--secondary);
        }

        .menu-card h3 {
            color: var(--secondary);
            margin-bottom: 0.8rem;
            font-family: 'Bangers', cursive;
            font-size: 1.5rem;
        }

        .menu-card ul {
            list-style-type: none;
        }

        .menu-card li {
            padding: 0.3rem 0;
            border-bottom: 1px dashed #334155;
        }

        /* Modal de Login */
        .modal {
            display: none;
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: rgba(0,0,0,0.8);
            justify-content: center;
            align-items: center;
            z-index: 2000;
        }

        .modal-content {
            background: var(--card-bg);
            padding: 2rem;
            border-radius: 12px;
            width: 100%;
            max-width: 400px;
            border: 2px solid var(--primary);
            text-align: center;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 1rem;
        }

        table th, table td {
            padding: 0.8rem;
            text-align: left;
            border-bottom: 1px solid #334155;
        }

        table th {
            background: #0f172a;
            color: var(--secondary);
        }

        footer {
            text-align: center;
            padding: 1.5rem;
            background: #0b1329;
            color: #94a3b8;
            font-size: 0.9rem;
            border-top: 2px solid #1e293b;
        }

        @media (max-width: 600px) {
            header h1 { font-size: 2.2rem; }
            nav { gap: 0.3rem; }
            nav button { padding: 0.4rem 0.6rem; font-size: 0.85rem; }
        }
    </style>
</head>
<body>

    <header>
        <h1>⚡ Vingadores Lego 2026 🧱</h1>
        <p>Junte-se à nossa Liga de Heróis para celebrar este aniversário épico!</p>
    </header>

    <nav>
        <button onclick="mudarPagina('home', this)" class="active"><i class="fa-solid fa-house"></i> Home</button>
        <button onclick="mudarPagina('cardapio', this)"><i class="fa-solid fa-pizza-slice"></i> Cardápio</button>
        <button onclick="mudarPagina('confirmar', this)"><i class="fa-solid fa-check-to-slot"></i> Confirmar</button>
        <button onclick="mudarPagina('cronograma', this)"><i class="fa-solid fa-clock"></i> Cronograma</button>
        <button onclick="mudarPagina('local', this)"><i class="fa-solid fa-map-location-dot"></i> Local</button>
        <button onclick="mudarPagina('avisos', this)"><i class="fa-solid fa-bullhorn"></i> Avisos</button>
        <button onclick="pedirSenhaAdmin()"><i class="fa-solid fa-gear"></i> Admin</button>
    </nav>

    <main>
        <!-- HOME -->
        <section id="page-home" class="page active">
            <h2><i class="fa-solid fa-shield-halved"></i> Missão: Aniversário Épico!</h2>
            <p>Convidados especiais, preparem suas pecinhas e superpoderes! Nosso herói favorita está completando mais um ano de vida e queremos você na nossa equipe para salvar o dia com muita diversão, brincadeiras e comidinhas deliciosas.</p>
            
            <div class="countdown-container">
                <div class="countdown-box"><span id="days">00</span><label>Dias</label></div>
                <div class="countdown-box"><span id="hours">00</span><label>Horas</label></div>
                <div class="countdown-box"><span id="minutes">00</span><label>Minutos</label></div>
                <div class="countdown-box"><span id="seconds">00</span><label>Segundos</label></div>
            </div>

            <div style="background: #0f172a; padding: 1.5rem; border-radius: 12px; margin-top: 1.5rem; border-left: 5px solid var(--primary);">
                <h3><i class="fa-solid fa-calendar-days"></i> Detalhes da Missão</h3>
                <p><strong>Data:</strong> 29 de Novembro de 2026</p>
                <p><strong>Horário:</strong> A partir das 15:00</p>
                <p><strong>Local:</strong> Salão de Festas MegaBlock - Rua dos Heróis, 123 - Rio de Janeiro - RJ</p>
            </div>
        </section>

        <!-- CARDÁPIO -->
        <section id="page-cardapio" class="page">
            <h2><i class="fa-solid fa-utensils"></i> Combates & Delícias (Buffet)</h2>
            <p>O quartel-general preparou um cardápio digno dos maiores heróis do universo Lego!</p>
            
            <div class="grid-menu">
                <div class="menu-card">
                    <h3>🍕 Salgados & Lanches</h3>
                    <ul>
                        <li>Mini Coxinhas do Homem de Ferro</li>
                        <li>Mini Pizzas do Capitão América</li>
                        <li>Batata Frita do Thor</li>
                        <li>Pão de Queijo do Hulk</li>
                    </ul>
                </div>
                <div class="menu-card">
                    <h3>🍰 Doces & Sobremesas</h3>
                    <ul>
                        <li>Bolo Temático Vingadores Lego</li>
                        <li>Cupcakes de Super-heróis</li>
                        <li>Brigadeiros Coloridos</li>
                        <li>Marshmallows</li>
                    </ul>
                </div>
                <div class="menu-card">
                    <h3>🥤 Bebidas do QG</h3>
                    <ul>
                        <li>Refrigerantes Variados</li>
                        <li>Sucos Naturais</li>
                        <li>Água Mineral</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- CONFIRMAR -->
        <section id="page-confirmar" class="page">
            <h2><i class="fa-solid fa-clipboard-user"></i> Confirmação de Presença (RSVP)</h2>
            <p>Confirme se sua equipe vai comparecer a esta grande missão!</p>
            
            <form id="form-rsvp" onsubmit="salvarConfirmacao(event)" style="margin-top: 1.5rem;">
                <div class="form-group">
                    <label>Nome do Convidado / Família:</label>
                    <input type="text" id="rsvp-nome" required placeholder="Ex: Família Silva">
                </div>
                <div class="form-group">
                    <label>Quantidade de Adultos:</label>
                    <input type="number" id="rsvp-adultos" min="0" value="1" required>
                </div>
                <div class="form-group">
                    <label>Quantidade de Crianças:</label>
                    <input type="number" id="rsvp-criancas" min="0" value="0" required>
                </div>
                <button type="submit" class="btn-action"><i class="fa-solid fa-paper-plane"></i> Enviar Confirmação</button>
            </form>
        </section>

        <!-- CRONOGRAMA -->
        <section id="page-cronograma" class="page">
            <h2><i class="fa-solid fa-clock"></i> Cronograma da Festa</h2>
            <div style="display: flex; flex-direction: column; gap: 1rem; margin-top: 1rem;">
                <div style="background: #0f172a; padding: 1rem; border-radius: 8px; border-left: 4px solid var(--secondary);">
                    <strong>15:00</strong> - Abertura dos Portões do QG (Chegada dos Convidados)
                </div>
                <div style="background: #0f172a; padding: 1rem; border-radius: 8px; border-left: 4px solid var(--primary);">
                    <strong>16:00</strong> - Oficinas de Montagem Lego & Brincadeiras com Super-heróis
                </div>
                <div style="background: #0f172a; padding: 1rem; border-radius: 8px; border-left: 4px solid var(--secondary);">
                    <strong>17:30</strong> - Hora do Parabéns e Corte do Bolo Épico!
                </div>
                <div style="background: #0f172a; padding: 1rem; border-radius: 8px; border-left: 4px solid var(--accent);">
                    <strong>19:00</strong> - Entrega das Lembrancinhas e Encerramento da Missão
                </div>
            </div>
        </section>

        <!-- LOCAL -->
        <section id="page-local" class="page">
            <h2><i class="fa-solid fa-map-location-dot"></i> Quartel-General</h2>
            <p>Onde a aventura vai acontecer:</p>
            <p style="margin: 1rem 0; font-weight: 600; color: var(--secondary);"><i class="fa-solid fa-location-dot"></i> Salão de Festas MegaBlock - Rua dos Heróis, 123 - Rio de Janeiro - RJ</p>
            <div style="border-radius: 12px; overflow: hidden; margin-top: 1rem; border: 2px solid var(--secondary);">
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3675.298!2d-43.35!3d-22.95!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zMjLCsDU3JzAwLjAiUyA0M8KwMjEnMDAuMCJX!5e0!3m2!1spt-BR!2sbr!4v1600000000000" width="100%" height="300" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
            </div>
        </section>

        <!-- AVISOS -->
        <section id="page-avisos" class="page">
            <h2><i class="fa-solid fa-bullhorn"></i> Mural de Avisos</h2>
            <div id="lista-avisos" style="margin-top: 1rem;">
                <div style="background: #0f172a; padding: 1rem; border-radius: 8px; margin-bottom: 0.8rem; border-left: 4px solid var(--secondary);">
                    <strong>Bem-vindos à Festa!</strong><br>
                    Não se esqueçam de confirmar presença na aba correspondente para ajudarmos na contagem dos kits de herói!
                </div>
            </div>
        </section>

        <!-- ADMIN -->
        <section id="page-admin" class="page">
            <h2><i class="fa-solid fa-gear"></i> Painel Administrativo</h2>
            <p>Lista oficial de heróis confirmados para o evento:</p>
            <div style="overflow-x: auto;">
                <table>
                    <thead>
                        <tr>
                            <th>Convidado</th>
                            <th>Adultos</th>
                            <th>Crianças</th>
                            <th>Ações</th>
                        </tr>
                    </thead>
                    <tbody id="tabela-convidados">
                        <!-- Preenchido via JS -->
                    </tbody>
                </table>
            </div>
            <button onclick="limparConvidados()" class="btn-action" style="background: #e63946; margin-top: 1.5rem;">Limpar Lista</button>
        </section>
    </main>

    <!-- Modal Senha Admin -->
    <div id="modal-admin" class="modal">
        <div class="modal-content">
            <h3>🔐 Acesso Restrito ao QG</h3>
            <p style="margin: 1rem 0; font-size: 0.9rem;">Digite a senha de Administrador:</p>
            <input type="password" id="senha-input" placeholder="Senha" style="margin-bottom: 1rem;">
            <button onclick="verificarSenhaAdmin()" class="btn-action">Entrar</button>
            <button onclick="fecharModalAdmin()" style="background: transparent; border: none; color: #94a3b8; margin-top: 0.8rem; cursor: pointer;">Cancelar</button>
        </div>
    </div>

    <footer>
        <p>&copy; 2026 Aniversário Vingadores Lego. Desenvolvido com poderes heroicos! ⚡🧱</p>
    </footer>

    <script>
        // Data do Evento: 29 de Novembro de 2026 às 15:00
        const EVENT_DATE = new Date('2026-11-29T15:00:00-03:00');
        const SENHA_ADMIN = 'admin2026';

        // Countdown
        function atualizarCountdown() {
            const now = new Date();
            const diff = EVENT_DATE - now;

            if (diff <= 0) {
                document.getElementById('days').innerText = '0';
                document.getElementById('hours').innerText = '0';
                document.getElementById('minutes').innerText = '0';
                document.getElementById('seconds').innerText = '0';
                return;
            }

            const days = Math.floor(diff / (1000 * 60 * 60 * 24));
            const hours = Math.floor((diff / (1000 * 60 * 60)) % 24);
            const minutes = Math.floor((diff / 1000 / 60) % 60);
            const seconds = Math.floor((diff / 1000) % 60);

            document.getElementById('days').innerText = String(days).padStart(2, '0');
            document.getElementById('hours').innerText = String(hours).padStart(2, '0');
            document.getElementById('minutes').innerText = String(minutes).padStart(2, '0');
            document.getElementById('seconds').innerText = String(seconds).padStart(2, '0');
        }
        setInterval(atualizarCountdown, 1000);
        atualizarCountdown();

        // Navegação de Páginas
        function mudarPagina(idPagina, btnEl) {
            document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
            document.getElementById('page-' + idPagina).classList.add('active');

            if(btnEl) {
                document.querySelectorAll('nav button').forEach(b => b.classList.remove('active'));
                btnEl.classList.add('active');
            }
        }

        // Sistema RSVP (LocalStorage)
        function salvarConfirmacao(e) {
            e.preventDefault();
            const nome = document.getElementById('rsvp-nome').value;
            const adultos = document.getElementById('rsvp-adultos').value;
            const criancas = document.getElementById('rsvp-criancas').value;

            let confirmados = JSON.parse(localStorage.getItem('legovingadores_rsvp') || '[]');
            confirmados.push({ nome, adultos, criancas, data: new Date().toLocaleDateString() });
            localStorage.setItem('legovingadores_rsvp', JSON.stringify(confirmados));

            alert('Presença confirmada com sucesso, herói! Sua equipe foi registrada.');
            document.getElementById('form-rsvp').reset();
            mudarPagina('home', document.querySelector('nav button'));
        }

        // Painel Admin
        function pedirSenhaAdmin() {
            document.getElementById('modal-admin').style.display = 'flex';
        }

        function fecharModalAdmin() {
            document.getElementById('modal-admin').style.display = 'none';
            document.getElementById('senha-input').value = '';
        }

        function verificarSenhaAdmin() {
            const senha = document.getElementById('senha-input').value;
            if (senha === SENHA_ADMIN) {
                fecharModalAdmin();
                carregarTabelaAdmin();
                document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
                document.getElementById('page-admin').classList.add('active');
            } else {
                alert('Senha incorreta!');
            }
        }

        function carregarTabelaAdmin() {
            const tbody = document.getElementById('tabela-convidados');
            let confirmados = JSON.parse(localStorage.getItem('legovingadores_rsvp') || '[]');
            
            tbody.innerHTML = '';
            if (confirmados.length === 0) {
                tbody.innerHTML = '<tr><td colspan="4" style="text-align: center; color: #94a3b8;">Nenhum convidado confirmado ainda.</td></tr>';
                return;
            }

            confirmados.forEach((item, index) => {
                tbody.innerHTML += `
                    <tr>
                        <td>${item.nome}</td>
                        <td>${item.adultos}</td>
                        <td>${item.criancas}</td>
                        <td><button onclick="removerConvidado(${index})" style="background: #e63946; color: white; border: none; padding: 0.3rem 0.6rem; border-radius: 4px; cursor: pointer;"><i class="fa-solid fa-trash"></i></button></td>
                    </tr>
                `;
            });
        }

        function removerConvidado(index) {
            let confirmados = JSON.parse(localStorage.getItem('legovingadores_rsvp') || '[]');
            confirmados.splice(index, 1);
            localStorage.setItem('legovingadores_rsvp', JSON.stringify(confirmados));
            carregarTabelaAdmin();
        }

        function limparConvidados() {
            if(confirm('Tem certeza que deseja apagar todos os convidados confirmados?')) {
                localStorage.removeItem('legovingadores_rsvp');
                carregarTabelaAdmin();
            }
        }
    </script>
</body>
</html>
