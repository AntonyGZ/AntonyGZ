---
layout: default
title: Antony Gomez
---

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');

body {
    background-color: #121212;
    color: #ffffff;
    font-family: 'Montserrat', sans-serif;
    margin: 0;
    padding: 0;
}

header {
    display: flex;
    align-items: center;
    padding: 20px;
    background-color: #1e1e1e;
    justify-content: space-between;
}

.profile-info {
    display: flex;
    align-items: center;
}

.profile-info img {
    width: 100px;
    border-radius: 50%;
    margin-right: 20px;
}

.nav-links {
    text-align: right;
}

.nav-links a {
    color: #f1c40f;
    margin-left: 15px;
    text-decoration: none;
    font-weight: bold;
}

.nav-links a:hover {
    text-decoration: underline;
}

.main {
    max-width: 900px;
    margin: 40px auto;
    padding: 0 20px;
}

h1, h2, h3 {
    color: #f1c40f;
}

section {
    margin-bottom: 50px;
}

.repo-container {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: center;
}

.repo-card {
    background-color: #1e1e1e;
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
    background-color: #1e1e1e;
    margin-top: 40px;
}

a {
    color: #f1c40f;
}

.social-links a {
    margin: 0 10px;
    color: #f1c40f;
    text-decoration: none;
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
    width: 50%;
    border-radius: 5px;
    border: none;
}

/* Estilo de los enlaces */
.nav-links a, .social-links a, .repo-card h3 a {
    color: #ffffff;
}

.nav-links a:hover, .social-links a:hover, .repo-card h3 a:hover, #repos-list a:hover, .post a:hover {
    color: #f1c40f;
}

/* Efectos para Post Destacados y Contacto y Redes Sociales */
.post a, .social-links a {
    color: #ffffff;
}

.post a:hover, .social-links a:hover {
    color: #000000;
}

/* Estilo para los videos */
.video-container {
    display: flex;
    gap: 10px;
    justify-content: space-between;
}

.video-container iframe {
    width: 48%;
    border-radius: 10px;
}

/* Estilo de iconos en el footer */
.footer-icons a {
    color: #f1c40f;
    margin: 0 10px;
}

.footer-icons a:hover {
    color: #ffffff;
}

</style>

<header>
    <div class="profile-info">
        <img src="https://github.com/AntonyGZ.png" alt="Foto de perfil">
        <div>
            <h1>Antony Gomez</h1>
            <p>Ingeniero de Sistemas | Desarrollador de Software | Entusiasta de la tecnología</p>
        </div>
    </div>
    <div class="nav-links">
        <a href="#home"><i class="fas fa-home"></i> Home</a>
        <a href="#about"><i class="fas fa-user"></i> About</a>
        <a href="#categories"><i class="fas fa-list"></i> Categories</a>
        <a href="#posts"><i class="fas fa-pen"></i> Posts</a>
    </div>
</header>

<main>
    <div class="search-box">
        <input type="text" placeholder="Buscar en la página...">
    </div>

    <section id="home">
        <h2>👋 Bienvenido</h2>
        <p>Hola, soy Antony Gómez. Estudiante de Ingeniería de Sistemas apasionado por la tecnología y la programación. Aquí comparto mis proyectos, ideas y aprendizajes. ¡Explora y conecta conmigo!</p>
    </section>

    <section id="about">
        <h2>📌 Sobre mí</h2>
        <div class="sub-box">
            <p>Me encuentro en constante aprendizaje, desarrollando proyectos personales y académicos relacionados con software, automatización y análisis técnico para trading. Estoy explorando el mundo del trading, con proyectos futuros donde podré compartir lo aprendido y ayudar a otros en su camino, todo con la visión de crecer profesionalmente en estos campos.</p>
        </div>
        <h3>🔗 Mi Interés en el Trading</h3>
        <div class="video-container">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/oxRcFzq10kQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            <iframe width="560" height="315" src="https://www.youtube.com/embed/d97JdIq4rmc" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
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
        <h2>🚀 Repositorios Destacados</h2>
        <div class="repo-container" id="repos-list">
            <p>Cargando repositorios...</p>
        </div>
        <p>👉 <a href="https://github.com/AntonyGZ?tab=repositories" target="_blank">Ver todos los repositorios</a></p>
    </section>

    <section id="contact">
        <h2>📬 Contacto y Redes Sociales</h2>
        <div class="social-links">
            <a href="https://github.com/AntonyGZ" target="_blank"><i class="fab fa-github"></i> GitHub</a>
            <a href="mailto:antonygomez0512@gmail.com"><i class="fas fa-envelope"></i> Email</a>
            <a href="https://wa.me/51991200117" target="_blank"><i class="fab fa-whatsapp"></i> WhatsApp</a>
            <a href="https://www.linkedin.com/in/antony-gomez-2b0155291/" target="_blank"><i class="fab fa-linkedin"></i> LinkedIn</a>
        </div>
    </section>
</main>

<footer>
    <div class="footer-icons">
        <a href="https://github.com/AntonyGZ" target="_blank"><i class="fab fa-github"></i></a>
        <a href="mailto:antonygomez0512@gmail.com"><i class="fas fa-envelope"></i></a>
        <a href="https://wa.me/51991200117" target="_blank"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.linkedin.com/in/antony-gomez-2b0155291/" target="_blank"><i class="fab fa-linkedin"></i></a>
    </div>
    <p>💡 Desarrollado con Jekyll y GitHub Pages por Antony Gomez</p>
</footer>

<script>
    async function loadRepos() {
        const response = await fetch('https://api.github.com/users/AntonyGZ/repos');
        const repos = await response.json();
        const reposList = document.getElementById('repos-list');
        reposList.innerHTML = '';

        repos.slice(0, 6).forEach(repo => {
            const div = document.createElement('div');
            div.className = 'repo-card';
            div.innerHTML = `
                <h3><a href="${repo.html_url}" target="_blank">${repo.name}</a></h3>
                <p>${repo.description || 'Sin descripción'}</p>
            `;
            reposList.appendChild(div);
        });
    }
    loadRepos();
</script>
