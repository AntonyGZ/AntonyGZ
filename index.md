---
layout: default
title: Antony Gomez
---

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;700&display=swap');
@import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css');

body {
    background-color: #121212;
    color: #ffffff;
    font-family: 'Inter', sans-serif;
    margin: 0;
    padding: 0;
}

nav {
    display: flex;
    justify-content: flex-end;
    background-color: #1e1e1e;
    padding: 15px 30px;
    position: sticky;
    top: 0;
    z-index: 100;
}

nav a {
    color: #f1c40f;
    margin-left: 20px;
    text-decoration: none;
    font-weight: 500;
}

nav a:hover {
    text-decoration: underline;
}

header {
    text-align: center;
    padding: 50px 20px 20px;
}

img {
    width: 150px;
    border-radius: 50%;
    margin-bottom: 10px;
    border: 3px solid #f1c40f;
}

h1, h2 {
    color: #f1c40f;
}

section {
    margin: 40px auto;
    max-width: 800px;
    text-align: center;
}

.repo-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
}

.repo-card {
    background-color: #1e1e1e;
    padding: 20px;
    border-radius: 10px;
    width: 250px;
    box-shadow: 0 4px 6px rgba(255, 255, 255, 0.1);
    transition: transform 0.3s ease;
    text-align: left;
}

.repo-card:hover {
    transform: translateY(-5px);
}

a {
    color: #f1c40f;
    text-decoration: none;
}

a:hover {
    text-decoration: underline;
}

footer {
    text-align: center;
    padding: 20px;
    background-color: #1e1e1e;
    margin-top: 40px;
}

.contact-icons {
    display: flex;
    justify-content: center;
    gap: 15px;
    margin-top: 15px;
}

.contact-icons a {
    color: #f1c40f;
    font-size: 24px;
}

.search-box {
    text-align: center;
    margin: 20px auto;
}

.search-box input {
    padding: 10px;
    border: none;
    border-radius: 5px;
    width: 300px;
    max-width: 80%;
}
</style>

<!-- Navbar -->
<nav>
    <a href="#home">Home</a>
    <a href="#tags">Tags</a>
    <a href="#about">About</a>
    <a href="#categorias">Categorías</a>
    <a href="#post">Post</a>
</nav>

<!-- Header -->
<header id="home">
    <img src="https://github.com/AntonyGZ.png" alt="Foto de perfil">
    <h1>👋 ¡Hola! Soy Antony Gomez</h1>
    <p>Bienvenido a mi página personal en GitHub Pages.</p>
    <div class="contact-icons">
        <a href="https://github.com/AntonyGZ" target="_blank"><i class="fab fa-github"></i></a>
        <a href="https://www.linkedin.com/in/antony-gomez-zuta/" target="_blank"><i class="fab fa-linkedin"></i></a>
        <a href="mailto:antonygomez.254@gmail.com"><i class="fas fa-envelope"></i></a>
        <a href="https://api.whatsapp.com/send?phone=51969604154" target="_blank"><i class="fab fa-whatsapp"></i></a>
    </div>
</header>

<!-- Search -->
<div class="search-box">
    <input type="text" placeholder="Buscar...">
</div>

<!-- About Section -->
<section id="about">
    <h2>📌 Sobre mí</h2>
    <p>Actualmente estudio Ingeniería de Sistemas y me apasiona el desarrollo de software. Aquí encontrarás algunos de mis proyectos y experimentos con código.</p>
</section>

<!-- Projects Section -->
<section id="categorias">
    <h2>🚀 Proyectos Destacados</h2>
    <div class="repo-container" id="repos-list">
        <p>Cargando repositorios...</p>
    </div>
    <p>👉 <a href="https://github.com/AntonyGZ?tab=repositories">Ver todos los repositorios</a></p>
</section>

<!-- Placeholder Sections -->
<section id="tags">
    <h2>🏷️ Tags</h2>
    <p>Aquí se mostrarán las etiquetas de tus proyectos o publicaciones.</p>
</section>

<section id="post">
    <h2>📝 Post</h2>
    <p>En esta sección puedes agregar tus artículos o publicaciones futuras.</p>
</section>

<!-- Footer -->
<footer>
    <p>💡 Desarrollado con Jekyll y GitHub Pages</p>
</footer>

<!-- Script to load repos -->
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
