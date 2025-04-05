---
layout: default
title: Antony Gomez
---

<head>
    <!-- Agregar Font Awesome para los íconos -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <!-- Agregar Google Fonts: Montserrat Regular -->
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400&display=swap" rel="stylesheet">
</head>

<style>
/* Cambiar la tipografía global a Montserrat Regular */
body {
    background: linear-gradient(135deg, #4E6B8E, #A1C4E8); /* Fondo profesional con gradiente */
    color: #ffffff;
    font-family: 'Montserrat', sans-serif; /* Aplicar Montserrat Regular a todo el cuerpo */
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
    margin-right: 50px; /* Asegurar espacio entre la imagen de perfil y el menú */
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
    padding-top: 160px; /* Ajustamos el contenido principal para que no se superponga al header */
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

/* Estilo para el cuadro adicional en la sección de "Acerca de mí" */
.sub-box {
    background-color: #34495e;
    padding: 15px;
    border-radius: 10px;
    margin-top: 20px;
}

/* Agregar un estilo de desplazamiento suave */
html {
    scroll-behavior: smooth;
}

/* Estilos para las pestañas con íconos */
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

/* Estilos de los títulos de los repositorios */
.repo-card h3 a {
    color: #f1c40f;
    text-decoration: none;
}

.repo-card h3 a:hover {
    color: #fff;
}

/* Estilo para los íconos de las pestañas */
.nav-links a:hover {
    color: #fff;
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

    <!-- Mover "Bienvenido" arriba -->
    <section id="home">
        <h2>👋 Bienvenido</h2>
        <p>Hola, soy Antony Gómez. Estudiante de Ingeniería de Sistemas apasionado por la tecnología y la programación. Aquí comparto mis proyectos, ideas y aprendizajes. ¡Explora y conecta conmigo!</p>
    </section>

    <section id="repos">
        <h2>🚀 Repositorios Destacados</h2>
        <div class="repo-container" id="repos-list">
            <!-- Los repositorios de GitHub se cargarán dinámicamente aquí -->
        </div>
        <p>👉 <a href="https://github.com/AntonyGZ?tab=repositories" target="_blank">Ver todos los repositorios</a></p>
    </section>

    <section id="about">
        <h2>📌 Sobre mí</h2>
        <p>Me encuentro en constante aprendizaje, desarrollando proyectos personales y académicos relacionados con software, automatización y análisis técnico para trading. Mi objetivo es crear soluciones prácticas y accesibles para usuarios y empresas.</p>

        <!-- Agregar la sección de Trading dentro de "Acerca de mí" -->
        <div class="sub-box">
            <h3>📊 Trading: Mi Interés</h3>
            <p>El análisis técnico y el trading son una de mis grandes pasiones. Actualmente, estoy estudiando estos temas y aplicando técnicas para tomar decisiones en el mercado financiero. A través de herramientas como gráficos y estadísticas, busco entender los patrones y las mejores oportunidades de inversión. ¡Espero seguir aprendiendo y compartir más sobre este emocionante campo!</p>
        </div>
    </section>

    <section id="categories">
        <h2>🗂️ Categorías</h2>
        <ul>
            <li><a href="#software">Desarrollo de Software</a></li>
            <li><a href="#trading">Análisis Técnico de Trading</a></li>
            <li><a href="#automacion">Automatización</a></li>
            <li><a href="#innovacion">Proyectos de Innovación</a></li>
        </ul>
    </section>

    <section id="posts">
        <h2>📝 Posts Destacados</h2>
        <div class="repo-container">
            <div class="repo-card">
                <h3><a href="#">Cómo empecé en el desarrollo web</a></h3>
                                <p>En este post comparto mi experiencia comenzando en el mundo del desarrollo web, las herramientas que utilicé, y cómo aprendí a construir aplicaciones web modernas.</p>
            </div>
            <div class="repo-card">
                <h3><a href="#">Introducción al análisis técnico</a></h3>
                <p>Un análisis profundo de cómo iniciarse en el análisis técnico para trading. Explico los principios básicos, patrones y herramientas más comunes utilizadas en los mercados financieros.</p>
            </div>
            <div class="repo-card">
                <h3><a href="#">Automatización con Python</a></h3>
                <p>Este post cubre los conceptos básicos de la automatización utilizando Python. Veremos ejemplos prácticos de cómo escribir scripts que realicen tareas de manera automática.</p>
            </div>
            <div class="repo-card">
                <h3><a href="#">Proyectos de Innovación y Tecnología</a></h3>
                <p>Un vistazo a proyectos de innovación que he desarrollado, con énfasis en cómo la tecnología puede transformar industrias tradicionales.</p>
            </div>
        </div>
    </section>

</main>

<footer>
    <p>&copy; 2025 Antony Gómez. Todos los derechos reservados.</p>
</footer>

<script>
    // Llenado de repositorios destacados
    const repos = [
        {
            name: "Sistema de Socios Mass",
            description: "Un sistema para gestionar los socios y promociones de una tienda.",
            link: "https://github.com/AntonyGZ/Sistema-Socios-Mass"
        },
        {
            name: "Trading Analysis Tool",
            description: "Una herramienta para realizar análisis técnico en el mercado financiero.",
            link: "https://github.com/AntonyGZ/Trading-Analysis-Tool"
        },
        {
            name: "Gestión de Tareas",
            description: "Aplicación para gestionar tareas personales y profesionales.",
            link: "https://github.com/AntonyGZ/Gestion-de-Tareas"
        },
        {
            name: "E-commerce App",
            description: "Una aplicación de comercio electrónico para gestionar productos y ventas.",
            link: "https://github.com/AntonyGZ/E-commerce-App"
        },
        {
            name: "Automatización con Python",
            description: "Un conjunto de scripts para automatizar tareas diarias en Python.",
            link: "https://github.com/AntonyGZ/Automatizacion-con-Python"
        },
        {
            name: "Blog de Tecnología",
            description: "Un blog donde comparto artículos sobre desarrollo de software, automatización, y más.",
            link: "https://github.com/AntonyGZ/Blog-de-Tecnologia"
        }
    ];

    const repoContainer = document.getElementById("repos-list");

    repos.forEach(repo => {
        const repoCard = document.createElement("div");
        repoCard.classList.add("repo-card");
        repoCard.innerHTML = `
            <h3><a href="${repo.link}" target="_blank">${repo.name}</a></h3>
            <p>${repo.description}</p>
        `;
        repoContainer.appendChild(repoCard);
    });
</script>

</body>
</html>
