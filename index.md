---
layout: default
title: Antony GZ
---

<header>
    <img src="https://github.com/AntonyGZ.png" alt="Foto de perfil" width="150" style="border-radius: 50%;">
    <h1>👋 ¡Hola! Soy Antony GZ</h1>
    <p>Bienvenido a mi página personal en GitHub Pages.</p>
</header>

<section>
    <h2>📌 Sobre mí</h2>
    <p>Actualmente estudio Ingeniería de Sistemas y me apasiona el desarrollo de software. Aquí encontrarás algunos de mis proyectos y experimentos con código.</p>
</section>

<section>
    <h2>🚀 Proyectos Destacados</h2>
    <ul id="repos-list">
        <li>Cargando repositorios...</li>
    </ul>
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

        repos.slice(0, 5).forEach(repo => {
            const li = document.createElement('li');
            li.innerHTML = `<a href="${repo.html_url}" target="_blank">${repo.name}</a>`;
            reposList.appendChild(li);
        });
    }
    loadRepos();
</script>
