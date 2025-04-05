---
layout: default
title: Antony Gomez
---

<head>
    <!-- Agregar Font Awesome para los íconos -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <!-- Tipografía moderna y profesional -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500&family=Inter:wght@400;600&display=swap" rel="stylesheet">
</head>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500&family=Inter:wght@400;600&display=swap'); /* Tipografía profesional */

body {
    background: linear-gradient(135deg, #4E6B8E, #A1C4E8); /* Fondo profesional con gradiente */
    color: #ffffff;
    font-family: 'Inter', sans-serif;
    margin: 0;
    padding: 0;
    min-height: 100vh;
}

header {
    display: flex;
    align-items: center;
    padding: 30px;
    background-color: #2c3e50;
    justify-content: space-between;
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 10;
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
    text-align: right;
}

.nav-links a {
    color: #f1c40f;
    margin-left: 20px;
    text-decoration: none;
    font-weight: bold;
}

.nav-links a:hover {
    text-decoration: underline;
}

main {
    width: 100%;
    max-width: 1200px;
    margin: 150px auto;
    padding: 0 20px;
}

h1, h2, h3 {
    color: #f1c40f;
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

/* Estilos Responsivos */
@media (max-width: 768px) {
    .nav-links {
        display: block;
        text-align: left;
    }

    .profile-info {
        max-width: 100%;
    }

    .repo-container {
        flex-direction: column;
        align-items: center;
    }
}

.video-container {
    display: flex;
    justify-content: space-between;
    gap: 20px;
    margin-top: 20px;
}

.video-container iframe {
    width: 48%;
    border-radius: 10px;
}
</style>

<header>
    <div class="profile-info">
        <img src="https://github.com/AntonyGZ.png" alt="Foto de perfil">
        <div>
            <h1>Antony Gomez</h1>
            <p>Ingeniero de Sistemas | Desarrollador de Software | Entusiasta de la tecnología</p>
            <!-- Redes sociales debajo de la foto -->
            <div class="social-links">
                <a href="https://github.com/AntonyGZ" target="_blank"><i class="fab fa-github"></i></a>
                <a href="mailto:antonygomez0512@gmail.com"><i class="fas fa-envelope"></i></a>
                <a href="https://wa.me/51991200117" target="_blank"><i class="fab fa-whatsapp"></i></a>
                <a href="https://www.linkedin.com/in/antony-gomez-2b0155291/" target="_blank"><i class="fab fa-linkedin"></i></a>
            </div>
        </div>
    </div>
    <div class="nav-links">
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#categories">Categories</a>
        <a href="#posts">Posts</a>
    </div>
</header>

<main>
    <div class="search-box">
        <input type="text" placeholder="Buscar en la página...">
    </div>

    <section id="repos">
        <h2>🚀 Repositorios Destacados</h2>
        <div class="repo-container" id="repos-list">
            <p>Cargando repositorios...</p>
        </div>
        <p>👉 <a href="https://github.com/AntonyGZ?tab=repositories" target="_blank">Ver todos los repositorios</a></p>
    </section>

    <section id="home">
        <h2>👋 Bienvenido</h2>
        <p>Hola, soy Antony Gómez. Estudiante de Ingeniería de Sistemas apasionado por la tecnología y la programación. Aquí comparto mis proyectos, ideas y aprendizajes. ¡Explora y conecta conmigo!</p>
    </section>

    <section id="about">
        <h2>📌 Sobre mí</h2>
        <p>Me encuentro en constante aprendizaje, desarrollando proyectos personales y académicos relacionados con software, automatización y análisis técnico para trading. Mi objetivo es crear soluciones prácticas y accesibles para usuarios y empresas.</p>
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

    <section id="trading">
        <h2>📊 Análisis Técnico y Trading</h2>
        <p>El análisis técnico y el trading son una de mis grandes pasiones. Actualmente, estoy estudiando estos temas y aplicando técnicas para tomar decisiones en el mercado financiero. A través de herramientas como gráficos y estadísticas, busco entender los patrones y las mejores oportunidades de inversión. ¡Espero seguir aprendiendo y compartir más sobre este emocionante campo!</p>
    </section>

    <section id="videos">
        <h2>📺 Videos sobre Trading</h2>
        <div class="video-container">
            <iframe src="https://www.youtube.com/embed/7qglzFYh0Jo" title="Video 1 sobre Trading" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            <iframe src="https://www.youtube.com/embed/kz-vjY9FGwI" title="Video 2 sobre Trading" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        </div>
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
            <a href="https://github.com/AntonyGZ" target="_blank"><i class="fab fa-github"></i> Git
