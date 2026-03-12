- 👋 Hi, I’m @Alphapellel624
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Alphapellel624/Alphapellel624 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your <?php
include("config.php");
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

:root {
    --primary-color: #667eea;
    --secondary-color: #764ba2;
    --text-color: #333;
    --light-bg: #f8f9fa;
    --white: #ffffff;
    --transition: all 0.3s ease;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: var(--text-color);
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* Navegación */
.navbar {
    background: var(--white);
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    position: sticky;
    top: 0;
    z-index: 1000;
}

.navbar .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 20px;
}

.logo {
    font-size: 1.5rem;
    font-weight: bold;
    color: var(--primary-color);
}

.nav-links {
    display: flex;
    list-style: none;
    gap: 2rem;
}

.nav-links a {
    text-decoration: none;
    color: var(--text-color);
    font-weight: 500;
    transition: var(--transition);
}

.nav-links a:hover {
    color: var(--primary-color);
}

/* Hero Section */
.hero {
    background: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%);
    color: var(--white);
    padding: 150px 20px;
    text-align: center;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
}

.hero-content h1 {
    font-size: 3.5rem;
    margin-bottom: 1rem;
    animation: slideUp 0.8s ease;
}

.hero-content p {
    font-size: 1.5rem;
    margin-bottom: 2rem;
    opacity: 0.9;
    animation: slideUp 0.8s ease 0.2s backwards;
}

@keyframes slideUp {
    from {
        opacity: 0;
        transform: translateY(30px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* Botones */
.btn {
    padding: 12px 30px;
    border: none;
    border-radius: 5px;
    font-size: 1rem;
    cursor: pointer;
    transition: var(--transition);
    text-decoration: none;
    display: inline-block;
}

.btn-primary {
    background: var(--primary-color);
    color: var(--white);
}

.btn-primary:hover {
    background: var(--secondary-color);
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
}

.btn-secondary {
    background: var(--light-bg);
    color: var(--primary-color);
    border: 2px solid var(--primary-color);
}

.btn-secondary:hover {
    background: var(--primary-color);
    color: var(--white);
}

/* Sección Sobre */
.about {
    padding: 80px 20px;
    background: var(--light-bg);
}

.about h2,
.projects h2,
.contact h2 {
    text-align: center;
    font-size: 2.5rem;
    margin-bottom: 3rem;
    color: var(--primary-color);
}

.about p {
    text-align: center;
    margin-bottom: 3rem;
    font-size: 1.1rem;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
}

.skills {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
    max-width: 900px;
    margin: 0 auto;
}

.skill h3 {
    margin-bottom: 0.5rem;
    color: var(--primary-color);
}

.progress {
    background: #e0e0e0;
    border-radius: 10px;
    height: 10px;
    overflow: hidden;
}

.progress-bar {
    background: linear-gradient(90deg, var(--primary-color), var(--secondary-color));
    height: 100%;
    border-radius: 10px;
    transition: width 1s ease;
}

/* Sección Proyectos */
.projects {
    padding: 80px 20px;
}

.projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
}

.project-card {
    background: var(--white);
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    transition: var(--transition);
}

.project-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 15px 30px rgba(0,0,0,0.2);
}

.project-image {
    height: 200px;
    background-size: cover;
}

.project-card h3,
.project-card p {
    padding: 0 1.5rem;
}

.project-card h3 {
    padding-top: 1.5rem;
    color: var(--primary-color);
}

.project-card p {
    padding-bottom: 1rem;
    color: #666;
}

.project-card .btn {
    margin: 0 1.5rem 1.5rem 1.5rem;
}

/* Sección Contacto */
.contact {
    padding: 80px 20px;
    background: var(--light-bg);
}

.contact p {
    text-align: center;
    margin-bottom: 2rem;
    font-size: 1.1rem;
}

.contact-form {
    max-width: 600px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    gap: 1rem;
}

.contact-form input,
.contact-form textarea {
    padding: 12px;
    border: 2px solid #ddd;
    border-radius: 5px;
    font-size: 1rem;
    font-family: inherit;
    transition: var(--transition);
}

.contact-form input:focus,
.contact-form textarea:focus {
    outline: none;
    border-color: var(--primary-color);
    box-shadow: 0 0 5px rgba(102, 126, 234, 0.3);
}

.contact-form button {
    margin-top: 0.5rem;
}

/* Footer */
.footer {
    background: #333;
    color: var(--white);
    padding: 2rem 20px;
    text-align: center;
}

.footer .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.social-links {
    display: flex;
    gap: 1.5rem;
}

.social-link {
    color: var(--white);
    text-decoration: none;
    transition: var(--transition);
}

.social-link:hover {
    color: var(--primary-color);
}

/* Responsivo */
@media (max-width: 768px) {
    .navbar .container {
        flex-direction: column;
        gap: 1rem;
    }

    .nav-links {
        gap: 1rem;
    }

    .hero-content h1 {
        font-size: 2rem;
    }

    .hero-content p {
        font-size: 1rem;
    }

    .footer .container {
        flex-direction: column;
        gap: 1rem;
    }
}
