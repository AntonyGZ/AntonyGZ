---
layout: default
title: "Antony GZ"
---

<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Antony GZ - Portfolio</title>
    <link rel="stylesheet" href="assets/css/style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
</head>
<body>
    <div class="container">
        <aside class="sidebar">
            <img src="assets/images/profile.jpg" alt="Antony GZ" class="profile-img">
            <h2>Antony GZ</h2>
            <p>Ingeniero de Sistemas | Desarrollador | Entusiasta de la Tecnología</p>
            <ul class="social-links">
                <li><i class="fas fa-map-marker-alt"></i> Tacna, Perú</li>
                <li><i class="fas fa-envelope"></i> <a href="mailto:correo@ejemplo.com">Email</a></li>
                <li><i class="fab fa-github"></i> <a href="https://github.com/AntonyGZ">GitHub</a></li>
                <li><i class="fab fa-linkedin"></i> <a href="#">LinkedIn</a></li>
            </ul>
        </aside>

        <main class="content">
            <header>
                <h1><i class="fas fa-code"></i> Antony GZ</h1>
                <nav>
                    <ul>
                        <li><a href="#">Home</a></li>
                        <li><a href="#">Categories</a></li>
                        <li><a href="#">Tags</a></li>
                        <li><a href="#">About</a></li>
                    </ul>
                </nav>
                <input type="text" id="search" placeholder="Buscar proyectos...">
            </header>
            
            <section id="projects">
                <h2>Mis Repositorios</h2>
                <div class="repo-list" id="repo-container"></div>
            </section>
        </main>
    </div>

    <script>
        fetch('https://api.github.com/users/AntonyGZ/repos')
            .then(response => response.json())
            .then(repos => {
                const container = document.getElementById('repo-container');
                repos.forEach(repo => {
                    const repoElement = document.createElement('div');
                    repoElement.classList.add('repo-card');
                    repoElement.innerHTML = `
                        <h3><a href="${repo.html_url}" target="_blank">${repo.name}</a></h3>
                        <p>${repo.description || 'Sin descripción'}</p>
                    `;
                    container.appendChild(repoElement);
                });
            });
    </script>
</body>
</html>
