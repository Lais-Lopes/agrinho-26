# agrinho-26<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Agro Forte, Futuro Sustentável</title>
    <style>
        /* Configurações Globais */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            color: #333;
            line-height: 1.6;
            background-color: #f9f9f9;
        }

        /* Cores Temáticas */
        :root {
            --verde-escuro: #1b4332;
            --verde-principal: #2d6a4f;
            --verde-claro: #52b788;
            --palha: #d8f3dc;
            --laranja-terra: #b7094c;
        }

        /* Cabeçalho e Navegação */
        header {
            background-color: var(--verde-escuro);
            color: white;
            padding: 1rem 5%;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 5px rgba(0,0,0,0.2);
        }

        header .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--verde-claro);
        }

        nav a {
            color: white;
            text-decoration: none;
            margin-left: 20px;
            transition: color 0.3s;
        }

        nav a:hover {
            color: var(--verde-claro);
        }

        /* Banner Principal (Hero) */
        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), 
                        url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?auto=format&fit=crop&w=1920&q=80') no-repeat center center/cover;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
            padding: 0 20px;
            margin-top: 60px;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.6);
        }

        .hero p {
            font-size: 1.5rem;
            max-width: 800px;
            margin-bottom: 30px;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.6);
        }

        .btn {
            background-color: var(--verde-claro);
            color: var(--verde-escuro);
            padding: 12px 30px;
            text-decoration: none;
            font-weight: bold;
            border-radius: 25px;
            transition: transform 0.3s, background-color 0.3s;
        }

        .btn:hover {
            background-color: white;
            transform: scale(1.05);
        }

        /* Seções Gerais */
        section {
            padding: 80px 10px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            color: var(--verde-escuro);
            margin-bottom: 50px;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 4px;
            background-color: var(--verde-claro);
            margin: 10px auto 0;
            border-radius: 2px;
        }

        /* Pilares (Cards) */
        .grid-pilares {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .card {
            background: white;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            border-top: 5px solid var(--verde-principal);
            transition: translateY 0.3s;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px rgba(0,0,0,0.1);
        }

        .card h3 {
            color: var(--verde-escuro);
            margin-bottom: 15px;
            font-size: 1.3rem;
        }

        /* Seção Sobre/Destaque */
        .sobre-container {
            display: flex;
            align-items: center;
            gap: 50px;
            flex-wrap: wrap;
        }

        .sobre-texto {
            flex: 1;
            min-width: 300px;
        }

        .sobre-texto p {
            margin-bottom: 20px;
            font-size: 1.1rem;
        }

        .sobre-img {
            flex: 1;
            min-width: 300px;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .sobre-img img {
            width: 100%;
            display: block;
        }

        /* Rodapé */
        footer {
            background-color: var(--verde-escuro);
            color: white;
            text-align: center;
            padding: 40px 20px;
            margin-top: 40px;
        }

        footer p {
            margin-bottom: 10px;
            font-size: 0.9rem;
        }

        /* Responsividade */
        @media (max-width: 768px) {
            .hero h1 { font-size: 2.2rem; }
            .hero p { font-size: 1.1rem; }
            header { flex-direction: column; text-align: center; gap: 10px; }
            nav a { margin: 0 10px; }
            .hero { margin-top: 100px; }
        }
    </style>
</head>
<body>

    <header>
        <div class="logo">AgroForte 🌱</div>
        <nav>
            <a href="#inicio">Início</a>
            <a href="#pilares">Pilares</a>
            <a href="#equilibrio">O Equilíbrio</a>
            <a href="#contato">Contato</a>
        </nav>
    </header>

    <div class="hero" id="inicio">
        <h1>Agro Forte, Futuro Sustentável</h1>
        <p>Alimentando o mundo hoje, garantindo a terra e os recursos para as próximas gerações através da tecnologia e do respeito ao meio ambiente.</p>
        <a href="#pilares" class="btn">Conheça Nossas Práticas</a>
    </div>

    <section id="pilares">
        <h2 class="section-title">Nossos Três Pilares</h2>
        <div class="grid-pilares">
            <div class="card">
                <h3>🚜 Alta Produtividade</h3>
                <p>Uso de tecnologias de precisão, inteligência artificial e biotecnologia para produzir mais alimentos por hectare, otimizando o uso do solo.</p>
            </div>
            <div class="card">
                <h3>💧 Preservação de Recursos</h3>
                <p>Sistemas avançados de irrigação gota a gota, manejo inteligente da água e proteção ativa de nascentes e matas ciliares.</p>
            </div>
            <div class="card">
                <h3>🔄 Economia Circular</h3>
                <p>Aproveitamento de resíduos agrícolas para a geração de bioenergia, adubação orgânica e redução drástica do desperdício no campo.</p>
            </div>
        </div>
    </section>

    <section id="equilibrio" style="background-color: #f0f7f4; max-width: 100%; width: 100%;">
        <div style="max-width: 1200px; margin: 0 auto; padding: 20px;">
            <h2 class="section-title">O Equilíbrio Perfeito</h2>
            <div class="sobre-container">
                <div class="sobre-texto">
                    <p>O grande desafio do século XXI não é apenas produzir, mas sim <strong>como produzir</strong>. Acreditamos que a força do agronegócio não caminha na direção oposta à preservação ambiental — elas andam de mãos dadas.</p>
                    <p>Através do plantio direto, rotação de culturas e a integração lavoura-pecuária-floresta (ILPF), conseguimos sequestrar carbono da atmosfera, recuperar solos degradados e manter a biodiversidade local enquanto batemos recordes de safra.</p>
                </div>
                <div class="sobre-img">
                    <img src="https://images.unsplash.com/photo-1625246333195-78d9c38ad451?auto=format&fit=crop&w=600&q=80" alt="Plantação sustentável e tecnologia">
                </div>
            </div>
        </div>
    </section>

    <footer id="contato">
        <p><strong>Agro Forte, Futuro Sustentável</strong></p>
        <p>Unindo força produtiva e consciência ecológica para cultivar o amanhã.</p>
        <p style="color: var(--verde-claro); margin-top: 20px;">© 2026 AgroForte. Todos os direitos reservados.</p>
    </footer>

</body>
</html>
