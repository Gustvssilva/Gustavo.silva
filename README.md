[Teste_portfolio_2.html](https://github.com/user-attachments/files/35225397/Teste_portfolio_2.html)

<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#101310">
<title>Gustavo Silva | Governança de TI</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Space+Grotesk:wght@400;500;600;700&display=swap" rel="stylesheet">

<style>
:root {
    --bg: #101310;
    --surface: #171c18;
    --surface2: #1d241e;
    --text: #edf0e9;
    --muted: #a0aaa0;
    --accent: #c2ed79;
    --border: #303a30;
    --max: 1120px;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html { scroll-behavior: smooth; }

body {
    background: var(--bg);
    color: var(--text);
    font-family: 'DM Sans', sans-serif;
    line-height: 1.7;
}

a {
    color: inherit;
    text-decoration: none;
}

.container {
    max-width: var(--max);
    margin: auto;
    padding: 0 28px;
}

header {
    position: sticky;
    top: 0;
    z-index: 100;
    background: rgba(16,19,16,.94);
    backdrop-filter: blur(15px);
    border-bottom: 1px solid var(--border);
}

.nav {
    max-width: var(--max);
    margin: auto;
    padding: 17px 28px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.logo {
    font-family: 'Space Grotesk';
    font-weight: 700;
    font-size: 21px;
}

.logo span { color: var(--accent); }

nav {
    display: flex;
    gap: 25px;
}

nav a {
    font-size: 13px;
    color: var(--muted);
    transition: .2s;
}

nav a:hover { color: var(--accent); }

.menu {
    display: none;
    background: none;
    color: var(--text);
    border: 1px solid var(--border);
    padding: 7px 12px;
    border-radius: 6px;
    cursor: pointer;
}

.hero {
    padding: 105px 0 75px;
    border-bottom: 1px solid var(--border);
}

.eyebrow {
    color: var(--accent);
    text-transform: uppercase;
    letter-spacing: 3px;
    font-size: 11px;
    font-weight: 700;
    margin-bottom: 22px;
}

.hero-grid {
    display: grid;
    grid-template-columns: 1fr 290px;
    align-items: center;
    gap: 55px;
}

h1, h2, h3 {
    font-family: 'Space Grotesk', sans-serif;
}

h1 {
    font-size: clamp(43px, 7vw, 76px);
    line-height: 1.06;
    letter-spacing: -3px;
    margin-bottom: 22px;
}

h1 span { color: var(--accent); }

.hero-description {
    max-width: 670px;
    color: var(--muted);
    font-size: 17px;
    margin-bottom: 28px;
}

.profile {
    width: 255px;
    height: 310px;
    object-fit: cover;
    border-radius: 15px;
    border: 1px solid var(--border);
    filter: saturate(.8);
}

.tags {
    display: flex;
    flex-wrap: wrap;
    gap: 9px;
    margin-bottom: 30px;
}

.tag {
    padding: 7px 13px;
    border: 1px solid var(--border);
    border-radius: 5px;
    font-size: 12px;
    color: var(--muted);
}

.actions {
    display: flex;
    gap: 13px;
    flex-wrap: wrap;
}

.btn {
    padding: 12px 21px;
    border-radius: 6px;
    font-size: 13px;
    font-weight: 700;
    display: inline-block;
    transition: .2s;
}

.btn-primary {
    background: var(--accent);
    color: #172013;
}

.btn-primary:hover { transform: translateY(-3px); }

.btn-outline {
    border: 1px solid var(--border);
}

.btn-outline:hover {
    border-color: var(--accent);
    color: var(--accent);
}

.stats {
    display: grid;
    grid-template-columns: repeat(3,1fr);
    gap: 20px;
    padding: 35px 0;
    border-bottom: 1px solid var(--border);
}

.stat strong {
    display: block;
    font-family: 'Space Grotesk';
    font-size: 32px;
    color: var(--accent);
}

.stat span {
    color: var(--muted);
    font-size: 12px;
}

section {
    padding: 90px 0;
    border-bottom: 1px solid var(--border);
}

.section-label {
    color: var(--accent);
    text-transform: uppercase;
    font-size: 11px;
    letter-spacing: 3px;
    margin-bottom: 10px;
}

.section-title {
    font-size: clamp(30px, 4vw, 43px);
    letter-spacing: -1.5px;
    margin-bottom: 20px;
}

.section-description {
    color: var(--muted);
    max-width: 720px;
    margin-bottom: 40px;
}

.about-grid {
    display: grid;
    grid-template-columns: 1.4fr 1fr;
    gap: 55px;
}

.about-text {
    color: var(--muted);
    font-size: 15px;
}

.about-text p { margin-bottom: 17px; }

.info {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 25px;
}

.info-item {
    padding: 13px 0;
    border-bottom: 1px solid var(--border);
}

.info-item:last-child { border: none; }

.info-item small {
    display: block;
    color: var(--muted);
    font-size: 11px;
    text-transform: uppercase;
    letter-spacing: 1px;
}

.info-item strong { font-size: 14px; }

.timeline {
    border-left: 1px solid var(--border);
    margin-left: 8px;
    padding-left: 30px;
}

.timeline-item {
    position: relative;
    margin-bottom: 40px;
}

.timeline-item::before {
    content: "";
    position: absolute;
    left: -36px;
    top: 8px;
    width: 11px;
    height: 11px;
    background: var(--accent);
    border-radius: 50%;
    box-shadow: 0 0 15px rgba(194,237,121,.3);
}

.date {
    color: var(--accent);
    font-size: 11px;
    letter-spacing: 1px;
    text-transform: uppercase;
}

.timeline h3 {
    font-size: 20px;
    margin: 6px 0;
}

.timeline p {
    color: var(--muted);
    font-size: 14px;
    max-width: 760px;
}

.cards {
    display: grid;
    grid-template-columns: repeat(2,1fr);
    gap: 18px;
}

.card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 10px;
    overflow: hidden;
    transition: .3s;
}

.card:hover {
    transform: translateY(-5px);
    border-color: var(--accent);
}

.card img {
    width: 100%;
    height: 215px;
    object-fit: cover;
    display: block;
}

.card-content { padding: 24px; }

.card h3 {
    font-size: 20px;
    margin-bottom: 10px;
}

.card p {
    color: var(--muted);
    font-size: 13px;
}

.card-category {
    color: var(--accent);
    font-size: 10px;
    letter-spacing: 2px;
    text-transform: uppercase;
    margin-bottom: 8px;
    display: block;
}

.skills-grid {
    display: grid;
    grid-template-columns: repeat(3,1fr);
    gap: 16px;
}

.skill-box {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 9px;
    padding: 23px;
}

.skill-box h3 {
    font-size: 17px;
    margin-bottom: 15px;
}

.skill-list {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
}

.skill {
    background: var(--surface2);
    color: var(--muted);
    padding: 6px 10px;
    font-size: 11px;
    border-radius: 4px;
}

.education {
    display: grid;
    grid-template-columns: repeat(2,1fr);
    gap: 17px;
}

.education-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 9px;
    padding: 24px;
}

.education-card span {
    color: var(--accent);
    font-size: 11px;
}

.education-card h3 {
    font-size: 18px;
    margin: 9px 0;
}

.education-card p {
    color: var(--muted);
    font-size: 13px;
}

.contact {
    text-align: center;
    padding: 100px 0;
}

.contact .section-description {
    margin: 0 auto 30px;
}

.contact-links {
    display: flex;
    justify-content: center;
    gap: 12px;
    flex-wrap: wrap;
}

footer {
    padding: 25px;
    text-align: center;
    color: var(--muted);
    font-size: 11px;
}

.reveal {
    opacity: 0;
    transform: translateY(22px);
    transition: opacity .7s ease, transform .7s ease;
}

.reveal.visible {
    opacity: 1;
    transform: translateY(0);
}

@media(max-width: 800px) {
    .hero-grid, .about-grid {
        grid-template-columns: 1fr;
    }

    .profile {
        width: 200px;
        height: 230px;
    }

    .skills-grid { grid-template-columns: repeat(2,1fr); }

    nav {
        display: none;
        position: absolute;
        top: 65px;
        left: 0;
        width: 100%;
        background: var(--surface);
        padding: 25px;
        flex-direction: column;
        gap: 18px;
        border-bottom: 1px solid var(--border);
    }

    nav.open { display: flex; }

    .menu { display: block; }
}

@media(max-width: 550px) {
    .cards, .education, .skills-grid {
        grid-template-columns: 1fr;
    }

    .stats { gap: 10px; }

    .stat strong { font-size: 25px; }

    .hero { padding-top: 65px; }

    section { padding: 65px 0; }

    h1 { letter-spacing: -2px; }
}

@media(prefers-reduced-motion: reduce) {
    *, *::before, *::after {
        scroll-behavior: auto !important;
        transition: none !important;
    }
    .reveal {
        opacity: 1;
        transform: none;
    }
}
</style>
</head>

<body>

<header>
    <div class="nav">
        <a href="#" class="logo">GUSTAVO<span>.</span></a>

        <nav id="navigation">
            <a href="#sobre">Sobre</a>
            <a href="#trajetoria">Trajetória</a>
            <a href="#projetos">Projetos</a>
            <a href="#habilidades">Habilidades</a>
            <a href="#formacao">Formação</a>
            <a href="#contato">Contato</a>
        </nav>

        <button class="menu" id="menuButton" aria-label="Abrir menu"
        aria-expanded="false">☰</button>
    </div>
</header>

<main>

<div class="container">
    <section class="hero">
        <div class="hero-grid">
            <div>
                <div class="eyebrow">Profissional do mercado financeiro</div>

                <h1>Gustavo<br><span>Silva.</span></h1>

                <p class="hero-description">
                    Governança de TI, controles internos e operações bancárias.
                    Conectando tecnologia, processos e visão de negócios
                    para gerar eficiência e resultados.
                </p>

                <div class="tags">
                    <span class="tag">Governança de TI</span>
                    <span class="tag">Middle Office</span>
                    <span class="tag">CPA-20</span>
                    <span class="tag">Power BI</span>
                    <span class="tag">VBA</span>
                </div>

                <div class="actions">
                    <a href="#trajetoria" class="btn btn-primary">Minha trajetória ↗</a>
                    <a href="#contato" class="btn btn-outline">Contato</a>
                </div>
            </div>

            <div>
                <img src="https://media.licdn.com/dms/image/v2/D4D03AQEfBNDMSk2odQ/profile-displayphoto-scale_400_400/B4DZ34on7lJYAg-/0/1777992893655?e=1796860800&v=beta&t=4mw8oZp2JCYj-9jhAlbZJ403UK23Ir3IjizenJRuKQY" alt="Gustavo Silva"
                class="profile">
            </div>
        </div>
    </section>

    <div class="stats">
        <div class="stat">
            <strong>5+</strong>
            <span>Anos no mercado financeiro</span>
        </div>
        <div class="stat">
            <strong>C-Pro R</strong>
            <span>Profissional certificado ANBIMA</span>
        </div>
        <div class="stat">
            <strong>2</strong>
            <span>Formações</span>
        </div>
    </div>

    <section id="sobre" class="reveal">
        <div class="section-label">Sobre mim</div>
        <h2 class="section-title">Tecnologia, processos e negócios.</h2>

        <div class="about-grid">
            <div class="about-text">
                <p>
                    Sou profissional do setor bancário, com aproximadamente
                    cinco anos de experiência no mercado financeiro e atuação
                    em Governança de TI e Middle Office.
                </p>

                <p>
                    Na área de Governança de TI, desenvolvi experiência em
                    suporte a auditorias, revisão de políticas internas,
                    gestão de controles, acompanhamento orçamentário,
                    administração de contratos e indicadores gerenciais.
                </p>

                <p>
                    Atualmente, atuo em operações bancárias, com experiência
                    em operações de câmbio, suporte a clientes e áreas
                    comerciais, processos de KYC, renovações de operações
                    financeiras e automação de atividades utilizando VBA.
                </p>

                <p>
                    Minha formação em Gestão da Tecnologia da Informação,
                    MBA em Gestão de TI e Projetos e certificação CPA-20
                    complementam minha visão analítica e de negócios.
                </p>

                <p>
                    Tenho interesse especial em governança, eficiência
                    operacional, controles internos e transformação digital.
                </p>
            </div>

            <div class="info">
                <div class="info-item">
                    <small>Área de interesse</small>
                    <strong>Governança de TI</strong>
                </div>
                <div class="info-item">
                    <small>Experiência</small>
                    <strong>Setor bancário</strong>
                </div>
                <div class="info-item">
                    <small>Certificação</small>
                    <strong>CPA-20</strong>
                </div>
                <div class="info-item">
                    <small>Ferramentas</small>
                    <strong>Excel, VBA e Power BI</strong>
                </div>
                <div class="info-item">
                    <small>Formação</small>
                    <strong>Gestão de TI e MBA</strong>
                </div>
                <div class="info-item">
                    <small>Idiomas</small>
                    <strong>Português e inglês</strong>
                </div>
            </div>
        </div>
    </section>

    <section id="trajetoria" class="reveal">
        <div class="section-label">Experiência profissional</div>
        <h2 class="section-title">Minha trajetória.</h2>

        <p class="section-description">
            Uma jornada construída no mercado financeiro, conectando
            tecnologia, governança e operações.
        </p>

        <div class="timeline">

            <div class="timeline-item">
                <span class="date">2021 — 2022</span>
                <h3>Estágio em Aplicações</h3>
                <p>
                    Início da trajetória profissional no ambiente de
                    tecnologia, com contato com sistemas corporativos,
                    processos e suporte às atividades da área de TI.
                </p>
            </div>

            <div class="timeline-item">
                <span class="date">2022 — 2025</span>
                <h3>Governança de TI | Banco Mizuho</h3>
                <p>
                    Atuação no suporte a auditorias, revisão de políticas
                    internas, controle orçamentário, gestão de fornecedores,
                    implantação de controles e elaboração de dashboards
                    e apresentações para a matriz e o board.
                </p>
            </div>

            <div class="timeline-item">
                <span class="date">2025 — Atual</span>
                <h3>Middle Office | Banco Mizuho</h3>
                <p>
                    Atuação em operações financeiras, câmbio, ACC/ACE,
                    renovações de operações, suporte a clientes e áreas
                    comerciais, KYC, controles operacionais e automações
                    utilizando VBA.
                </p>
            </div>

            <div class="timeline-item">
                <span class="date">Próximo capítulo</span>
                <h3>Governança, tecnologia e eficiência</h3>
                <p>
                    Desenvolvimento contínuo em governança corporativa
                    de TI, gestão de riscos, controles internos,
                    indicadores e melhoria de processos.
                </p>
            </div>

        </div>
    </section>

    <section id="projetos" class="reveal">
        <div class="section-label">experiências</div>
        <h2 class="section-title">Resultados na prática.</h2>

        <p class="section-description">
            Projetos e iniciativas relacionados à tecnologia,
            gestão e eficiência operacional.
        </p>

        <div class="cards">

            <article class="card">
                <img src="https://lec.com.br/wp-content/uploads/2020/07/18771-scaled-1.jpg"
                alt="Projeto de governança">
                <div class="card-content">
                    <span class="card-category">Governança de TI</span>
                    <h3>Controles e Governança</h3>
                    <p>
                        Participação na estruturação e acompanhamento
                        de controles internos, suporte a auditorias
                        e revisão de políticas corporativas.
                    </p>
                </div>
            </article>

            <article class="card">
                <img src="https://files.sunoresearch.com.br/p/uploads/2020/08/corporate-banking-1024x676.jpg"
                alt="Projeto de tecnologia">
                <div class="card-content">
                    <span class="card-category">Middle Office</span>
                    <h3>Operações financeiras Onshore & Offshore </h3>
                    <p>
                        Experiência na distribuição de produtos de 
                        crédito e câmbio e no suporte à operações Onshore & Offshore.
                    </p>
                </div>
            </article>

        </div>
    </section>

    <section id="habilidades" class="reveal">
        <div class="section-label">Competências</div>
        <h2 class="section-title">Conhecimentos e habilidades.</h2>

        <p class="section-description">
            Competências desenvolvidas ao longo da experiência
            profissional e formação acadêmica.
        </p>

        <div class="skills-grid">

            <div class="skill-box">
                <h3>Governança e Gestão</h3>
                <div class="skill-list">
                    <span class="skill">Governança de TI</span>
                    <span class="skill">Auditoria</span>
                    <span class="skill">Controles internos</span>
                    <span class="skill">Gestão de riscos</span>
                    <span class="skill">Políticas internas</span>
                    <span class="skill">Gestão de fornecedores</span>
                </div>
            </div>

            <div class="skill-box">
                <h3>Dados e Automação</h3>
                <div class="skill-list">
                    <span class="skill">Excel</span>
                    <span class="skill">VBA</span>
                    <span class="skill">Power BI</span>
                    <span class="skill">Dashboards</span>
                    <span class="skill">Indicadores</span>
                    <span class="skill">IA</span>
                </div>
            </div>

            <div class="skill-box">
                <h3>Mercado Financeiro</h3>
                <div class="skill-list">
                    <span class="skill">Middle Office</span>
                    <span class="skill">KYC</span>
                    <span class="skill">Câmbio</span>
                    <span class="skill">ACC / ACE</span>
                    <span class="skill">SWIFT</span>
                    <span class="skill">CPA-20</span>
                </div>
            </div>

        </div>
    </section>

    <section id="formacao" class="reveal">
        <div class="section-label">Formação acadêmica</div>
        <h2 class="section-title">Conhecimento em evolução.</h2>

        <div class="education">

            <div class="education-card">
                <span>FIAP</span>
                <h3>MBA em Gestão de TI e Projetos</h3>
                <p>Formação em gestão de tecnologia,
                projetos e estratégia.</p>
            </div>

            <div class="education-card">
                <span>FIAP</span>
                <h3>Gestão da Tecnologia da Informação</h3>
                <p>Formação superior em tecnologia,
                processos e gestão.</p>
            </div>

            <div class="education-card">
                <span>Saint Paul</span>
                <h3>Operador / Banker</h3>
                <p>Formação voltada ao mercado financeiro.</p>
            </div>

            <div class="education-card">
                <span>Certificações e idiomas</span>
                <h3>CPA-20 e TOEIC</h3>
                <p>CPA-20 ANBIMA e certificações
                de proficiência em inglês.</p>
            </div>

        </div>
    </section>

    <section id="contato" class="contact reveal">
        <div class="section-label">Contato</div>
        <h2 class="section-title">Vamos nos conectar?</h2>

        <p class="section-description">
            Estou aberto a conexões profissionais e oportunidades
            relacionadas à governança de TI, tecnologia,
            controles internos e mercado financeiro.
        </p>

        <div class="contact-links">
            <a class="btn btn-primary"
            href="mailto:gustavo.silva.ti3@gmail.com">
                Enviar e-mail ↗
            </a>

            <a class="btn btn-outline"
            href="https://www.linkedin.com/in/gustavo-silva-ab007a192"
            target="_blank" rel="noopener noreferrer">
                LinkedIn ↗
            </a>

            <a class="btn btn-outline"
            href="https://github.com/Gustvssilva"
            target="_blank" rel="noopener noreferrer">
                GitHub ↗
            </a>
        </div>
    </section>
</div>
</main>

<footer>
    © 2026 Gustavo Silva · Todos os direitos reservados.
</footer>

<script>
const menuButton = document.getElementById('menuButton');
const navigation = document.getElementById('navigation');

menuButton.addEventListener('click', () => {
    const opened = navigation.classList.toggle('open');
    menuButton.setAttribute('aria-expanded', opened);
});

document.querySelectorAll('#navigation a').forEach(link => {
    link.addEventListener('click', () => {
        navigation.classList.remove('open');
        menuButton.setAttribute('aria-expanded', 'false');
    });
});

const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
        if (entry.isIntersecting) {
            entry.target.classList.add('visible');
            observer.unobserve(entry.target);
        }
    });
}, { threshold: 0.12 });

document.querySelectorAll('.reveal').forEach(element => {
    observer.observe(element);
});
</script>

</body>
</html>
