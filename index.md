---
layout: default
title: Antony Gomez
---

<style>
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;700&display=swap');

body {
    font-family: 'Inter', sans-serif;
}
    body {
        background-color: #121212;
        color: #ffffff;
        font-family: Arial, sans-serif;
        text-align: center;
        margin: 0;
        padding: 0;
    }
    header {
        padding: 50px 20px;
    }
    img {
        width: 150px;
        border-radius: 50%;
        margin-bottom: 10px;
    }
    h1, h2 {
        color: #f1c40f;
    }
    section {
        margin: 40px auto;
        max-width: 800px;
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
</style>

<header>
    <img src="https://github.com/AntonyGZ.png" alt="Foto de perfil">
    <h1>👋 ¡Hola! Soy Antony GZ</h1>
    <p>Bienvenido a mi página personal en GitHub Pages.</p>
</header>

<section>
    <h2>📌 Sobre mí</h2>
    <p>Actualmente estudio Ingeniería de Sistemas y me apasiona el desarrollo de software. Aquí encontrarás algunos de mis proyectos y experimentos con código.</p>
</section>

<section>
    <h2>🚀 Proyectos Destacados</h2>
    <div class="repo-container" id="repos-list">
        <p>Cargando repositorios...</p>
    </div>
    <p>👉 <a href="https://github.com/AntonyGZ?tab=repositories">Ver todos los repositorios</a></p>
</section>

<footer>
    <p>💡 Desarrollado con Jekyll y GitHub Pages</p>
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
