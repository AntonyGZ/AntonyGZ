---
layout: default
title: Antony Gomez
---

<style>
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;700&display=swap');

    body {
        background-color: #121212;
        color: #ffffff;
        font-family: 'Inter', sans-serif;
        text-align: center;
        margin: 0;
        padding: 0;
        line-height: 1.6;
    }

    header {
        padding: 50px 20px;
        animation: fadeIn 1s ease-out;
    }

    img {
        width: 150px;
        border-radius: 50%;
        margin-bottom: 10px;
        border: 3px solid #f1c40f;
        transition: transform 0.3s ease;
    }

    img:hover {
        transform: scale(1.05);
    }

    h1, h2 {
        color: #f1c40f;
        margin-bottom: 10px;
    }

    section {
        margin: 40px auto;
        max-width: 800px;
        padding: 0 20px;
    }

    .repo-container {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 20px;
        animation: fadeIn 1.5s ease-out;
    }

    .repo-card {
        background-color: #1e1e1e;
        padding: 20px;
        border-radius: 10px;
        width: 250px;
        box-shadow: 0 4px 12px rgba(241, 196, 15, 0.2);
        transition: transform 0.3s ease, box-shadow 0.3s ease;
        text-align: left;
    }

    .repo-card:hover {
        transform: translateY(-5px);
        box-shadow: 0 8px 16px rgba(241, 196, 15, 0.4);
    }

    a {
        color: #f1c40f;
        text-decoration: none;
        transition: color 0.3s ease;
    }

    a:hover {
        text-decoration: underline;
        color: #f39c12;
    }

    footer {
        margin-top: 50px;
        padding: 20px;
        background-color: #1e1e1e;
        color: #777;
    }

    /* Animaciones */
    @keyframes fadeIn {
        from { opacity: 0; transform: translateY(20px); }
        to { opacity: 1; transform: translateY(0); }
    }
</style>

<header>
    <img src="https://github.com/AntonyGZ.png" alt="Foto de perfil">
    <h1>👋 ¡Hola! Soy Antony Gomez</h1>
    <p>Bienvenido a mi página personal en GitHub Pages.</p>
</header>

<section>
    <h2>📌 Sobre mí</h2>
    <p>Actualmente estudio Ingeniería de Sistemas y me apasiona el desarrollo de software. Aquí encontrarás algunos de mis proyectos y experimentos con código.</p>
</section>

<section>
    <h2>🚀 Proyectos Destacados</h2>
    <div class="repo-container" id="repos-list">
        <p>🔄 Cargando repositorios...</p>
    </div>
    <p>👉 <a href="https://github.com/AntonyGZ?tab=repositories">Ver todos los repositorios</a></p>
</section>

<footer>
    <p>💡 Desarrollado con Jekyll y GitHub Pages</p>
</footer>

<script>
    async function loadRepos() {
        try {
            const response = await fetch('https://api.github.com/users/AntonyGZ/repos');
            const repos = await response.json();
            const reposList = document.getElementById('repos-list');
            reposList.innerHTML = '';

            repos
                .sort((a, b) => b.stargazers_count - a.stargazers_count) // ordena por estrellas
                .slice(0, 6) // muestra solo los 6 primeros
                .forEach(repo => {
                    const div = document.createElement('div');
                    div.className = 'repo-card';
                    div.innerHTML = `
                        <h3><a href="${repo.html_url}" target="_blank">${repo.name}</a></h3>
                        <p>${repo.description ? repo.description : 'Sin descripción disponible.'}</p>
                        <p>⭐ ${repo.stargazers_count} | 🍴 ${repo.forks_count}</p>
                    `;
                    reposList.appendChild(div);
                });

            if (reposList.innerHTML.trim() === '') {
                reposList.innerHTML = '<p>No se encontraron repositorios.</p>';
            }
        } catch (error) {
            console.error('Error al cargar repositorios:', error);
            document.getElementById('repos-list').innerHTML = '<p>⚠️ Error al cargar los repositorios.</p>';
        }
    }

    loadRepos();
</script>
