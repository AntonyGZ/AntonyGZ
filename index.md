---
layout: default
title: Antony Gomez
---

<head>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400&display=swap" rel="stylesheet">
</head>

<style>
body {
    background: linear-gradient(135deg, #4E6B8E, #A1C4E8);
    color: #ffffff;
    font-family: 'Montserrat', sans-serif;
    margin: 0;
    padding: 0;
    min-height: 100vh;
}

header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 30px;
    background-color: #2c3e50;
    width: 100%;
    z-index: 10;
    box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.5);
    position: relative;
}

.profile-info {
    display: flex;
    align-items: center;
    flex-direction: column;
    text-align: center;
    max-width: 300px;
    margin-right: 50px;
}

.profile-info img {
    width: 120px;
    border-radius: 50%;
    margin-bottom: 20px;
}

.profile-info h1 {
    margin: 0;
    font-size: 2.5em;
    color: #f1c40f;
}

.profile-info p {
    font-size: 1.2em;
}

.social-links a {
    margin: 0 10px;
    color: #f1c40f;
    text-decoration: none;
    font-size: 1.5em;
}

.social-links a:hover {
    color: #fff;
}

.nav-links {
    display: flex;
    align-items: center;
    gap: 20px;
    font-weight: bold;
}

.nav-links a {
    color: #f1c40f;
    text-decoration: none;
}

.nav-links a:hover {
    text-decoration: underline;
}

main {
    padding-top: 160px;
}

section {
    background-color: rgba(0, 0, 0, 0.7);
    margin-bottom: 40px;
    padding: 20px;
    border-radius: 10px;
}

section h2 {
    margin-top: 0;
}

.repo-container {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: center;
}

.repo-card {
    background-color: #34495e;
    padding: 20px;
    border-radius: 10px;
    width: 250px;
    box-shadow: 0 4px 6px rgba(255, 255, 255, 0.1);
    transition: transform 0.3s ease;
}

.repo-card:hover {
    transform: translateY(-5px);
}

footer {
    text-align: center;
    padding: 20px;
    background-color: #2c3e50;
    margin-top: 40px;
    color: #fff;
}

a {
    color: #f1c40f;
}

.social-links a {
    margin: 0 10px;
    color: #f1c40f;
    text-decoration: none;
    font-size: 1.5em;
}

.social-links a:hover {
    text-decoration: underline;
}

.search-box {
    text-align: center;
    margin-bottom: 30px;
}

input[type="text"] {
    padding: 10px;
    width: 60%;
    border-radius: 5px;
    border: none;
    font-size: 1em;
}

.sub-box {
    background-color: #34495e;
    padding: 15px;
    border-radius: 10px;
    margin-top: 20px;
}

html {
    scroll-behavior: smooth;
}

.nav-links a {
    font-size: 1.2em;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.nav-links a i {
    font-size: 2em;
    margin-bottom: 5px;
}

.repo-card h3 a {
    color: #f1c40f;
    text-decoration: none;
}

.repo-card h3 a:hover {
    color: #fff;
}

.nav-links a:hover {
    color: #fff;
}

footer .social-links {
    margin-top: 20px;
}

footer .social-links a {
    margin: 0 10px;
    color: #f1c40f;
    font-size: 1.5em;
}

footer .social-links a:hover {
    color: #fff;
}

</style>

<header>
    <div class="profile-info">
        <img src="https://github.com/AntonyGZ.png" alt="Foto de perfil">
        <div>
            <h1>Antony Gomez</h1>
            <p>Ingeniero de Sistemas | Desarrollador de Software | Entusiasta de la tecnología</p>
            <div class="social-links">
                <a href="https://github.com/AntonyGZ" target="_blank"><i class="fab fa-github"></i></a>
                <a href="mailto:60450594@continental.edu.pe"><i class="fas fa-envelope"></i></a>
                <a href="https://wa.me/51991200117" target="_blank"><i class="fab fa-whatsapp"></i></a>
                <a href="https://www.linkedin.com/in/antony-gomez-2b0155291/" target="_blank"><i class="fab fa-linkedin"></i></a>
            </div>
        </div>
    </div>
    <div class="nav-links">
        <a href="#home"><i class="fas fa-home"></i> Home</a>
        <a href="#categories"><i class="fas fa-th"></i> Categories</a>
        <a href="#about"><i class="fas fa-user"></i> About</a>
        <a href="#posts"><i class="fas fa-file-alt"></i> Posts</a>
    </div>
</header>

<main>
    <div class="search-box">
        <input type="text" placeholder="Buscar en la página...">
    </div>

    <section id="repos">
        <h2>🚀 Repositorios Destacados</h2>
        <div class="repo-container" id="repos-list">
        </div>
        <p>👉 <a href="https://github.com/AntonyGZ?tab=repositories" target="_blank">Ver todos los repositorios</a></p>
    </section>

    <section id="home">
        <h2>👋 Bienvenido</h2>
        <p>Hola, soy Antony Gómez. Estudiante de Ingeniería de Sistemas apasionado por la tecnología y la programación. Aquí comparto mis proyectos, ideas y aprendizajes. ¡Explora y conecta conmigo!</p>
    </section>

    <section id="about">
        <h2>📌 Sobre mí</h2>
        <p>Soy estudiante de Ingeniería en Sistemas con una pasión por el desarrollo de software y la programación. Me encanta enfrentarme a nuevos desafíos tecnológicos, y me esfuerzo constantemente por expandir mis conocimientos en este fascinante mundo digital.
Mi enfoque principal es la creación de soluciones innovadoras a través de código, pero también soy un entusiasta del trading, un campo que he comenzado a explorar con curiosidad y dedicación. A través del aprendizaje continuo, estoy perfeccionando mis habilidades para comprender y aplicar estrategias financieras, lo que me permite combinar mi pasión por la tecnología con nuevas oportunidades de crecimiento profesional.
Mi objetivo es colaborar con personas que también estén interesadas en aprender y desarrollar juntos, enfrentando proyectos que nos permitan crecer como profesionales, compartir ideas y construir soluciones que realmente marquen la diferencia. Si buscas a alguien comprometido, curioso y con muchas ganas de aprender y enseñar, ¡me encantaría conectar contigo!</p>

        <div class="sub-box">
            <h3>📊 Trading: Mi Interés</h3>
            <p>El análisis técnico y el trading son una de mis grandes pasiones. Actualmente, estoy estudiando estos temas y aplicando técnicas para tomar decisiones en el mercado financiero. A través de herramientas como gráficos y estadísticas, busco entender los patrones y las mejores oportunidades de inversión. ¡Espero seguir aprendiendo y compartir más sobre este emocionante campo!</p>

            <div class="video-container">
                <iframe src="https://www.youtube.com/embed/oxRcFzq10kQ" title="Video 1 sobre Trading" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <iframe src="https://www.youtube.com/embed/d97JdIq4rmc" title="Video 2 sobre Trading" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </div>
        </div>
    </section>

    <section id="categories">
        <h2>🗂️ Categorías</h2>
        <ul>
            <li>Desarrollo de Software</li>
            <li>Análisis Técnico de Trading</li>
            <li>Automatización</li>
            <li>Proyectos de Innovación</li>
        </ul>
    </section>

    <section id="posts">
        <h2>📝 Posts Destacados</h2>
        <ul>
            <li><a href="#">Cómo empecé en el desarrollo web</a></li>
            <li><a href="#">Proyectos académicos que marcaron mi camino</a></li>
            <li><a href="#">Mis herramientas favoritas para desarrollo y análisis</a></li>
        </ul>
    </section>

    <section>
        <h2>📬 Contacto y Redes Sociales</h2>
        <div class="social-links">
            <a href="https://github.com/AntonyGZ" target="_blank"><i class="fab fa-github"></i></a>
            <a href="mailto:antonygomez0512@gmail.com"><i class="fas fa-envelope"></i></a>
            <a href="https://wa.me/51991200117" target="_blank"><i class="fab fa-whatsapp"></i></a>
            <a href="https://www.linkedin.com/in/antony-gomez-2b0155291/" target="_blank"><i class="fab fa-linkedin"></i></a>
        </div>
    </section>
</main>

<footer>
    <p>&copy; 2025 Antony Gomez. Todos los derechos reservados.</p>
</footer>

<script>
    fetch('https://api.github.com/users/AntonyGZ/')
        .then(response => response.json())
        .then(data => {
            const reposList = document.getElementById('repos-list');
            data.forEach(repo => {
                const repoCard = document.createElement('div');
                repoCard.className = 'repo-card';
                repoCard.innerHTML = `
                    <h3><a href="${repo.html_url}" target="_blank">${repo.name}</a></h3>
                    <p>${repo.description ||}</p>
                `;
                reposList.appendChild(repoCard);
            });
        })
        .catch(error => console.log('Error fetching repositories:', error));
</script>
