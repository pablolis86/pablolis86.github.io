<html><head><base href="." /><meta charset="UTF-8" /><meta name="viewport" content="width=device-width, initial-scale=1.0" /><title>UNLu Consulting Group - Consultora de Negocios</title><style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
  }

  :root {
    --primary: #1a4f8b;
    --secondary: #2980b9;
    --accent: #f39c12;
    --light: #ecf0f1;
    --dark: #2c3e50;
  }

  body {
    overflow-x: hidden;
    padding-top: 70px;
  }

  nav {
    padding: 1.5rem 10%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: var(--primary);
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 1000;
    box-shadow: 0 2px 10px rgba(0,0,0,0.1);
  }


h1, .site-title {
    display: none;
}


  .header {
    background: linear-gradient(rgba(26, 79, 139, 0.95), rgba(26, 79, 139, 0.95)), url('https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?ixlib=rb-4.0.3') center/cover;
    height: 100vh;
    color: white;
    display: flex;
    flex-direction: column;
  }

  .logo {
    font-size: 1.8rem;
    font-weight: 700;
    color: var(--light);
  }

  .nav-links {
    display: flex;
    gap: 2rem;
  }

  .nav-links a {
    color: var(--light);
    text-decoration: none;
    font-weight: 500;
    transition: color 0.3s;
  }

  .nav-links a:hover {
    color: var(--accent);
  }

  .mobile-menu-btn {
    display: none;
    font-size: 1.5rem;
    color: var(--light);
    background: none;
    border: none;
    cursor: pointer;
  }

  .hero {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 0 10%;
  }

  .hero h2 {
    font-size: 3.5rem;
    margin-bottom: 1rem;
  }

  .hero p {
    font-size: 1.2rem;
    margin-bottom: 2rem;
  }

  .cta-button {
    background: var(--accent);
    color: white;
    padding: 1rem 2rem;
    border-radius: 30px;
    text-decoration: none;
    font-weight: 600;
    transition: transform 0.3s;
  }

  .cta-button:hover {
    transform: scale(1.05);
  }

  .services {
    padding: 5rem 10%;
    background: var(--light);
  }

  .section-title {
    text-align: center;
    margin-bottom: 3rem;
    color: var(--dark);
  }

  .services-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
  }

  .service-card {
    background: white;
    padding: 2rem;
    border-radius: 10px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    transition: transform 0.3s;
  }

  .service-card:hover {
    transform: translateY(-10px);
  }

  .service-icon {
    font-size: 2.5rem;
    color: var(--primary);
    margin-bottom: 1rem;
  }

  .team {
    padding: 5rem 10%;
    background: white;
  }

  .team-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
    margin-top: 3rem;
  }

  .team-member {
    text-align: center;
    padding: 2rem;
    border-radius: 10px;
    background: var(--light);
    transition: transform 0.3s;
  }

  .team-member:hover {
    transform: translateY(-10px);
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  }

  .team-member .avatar {
    width: 150px;
    height: 150px;
    background: var(--primary);
    border-radius: 50%;
    margin: 0 auto 1.5rem;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .team-member .avatar i {
    font-size: 4rem;
    color: white;
  }

  .contact {
    padding: 5rem 10%;
    background: var(--dark);
    color: white;
  }

  .contact-form {
    max-width: 600px;
    margin: 0 auto;
  }

  .form-group {
    margin-bottom: 1.5rem;
  }

  .form-group input,
  .form-group textarea {
    width: 100%;
    padding: 0.8rem;
    border: none;
    border-radius: 5px;
    margin-top: 0.5rem;
  }

  .submit-btn {
    background: var(--accent);
    color: white;
    border: none;
    padding: 1rem 2rem;
    border-radius: 5px;
    cursor: pointer;
    width: 100%;
    font-size: 1rem;
    font-weight: 600;
  }

  footer {
    background: var(--primary);
    color: white;
    text-align: center;
    padding: 2rem;
  }

  @media (max-width: 768px) {
    nav {
      padding: 1rem 5%;
    }

    .logo {
      font-size: 1.4rem;
    }

    .mobile-menu-btn {
      display: block;
    }

    .nav-links {
      display: none;
      position: absolute;
      top: 100%;
      left: 0;
      right: 0;
      background: var(--primary);
      flex-direction: column;
      padding: 1rem 0;
      gap: 1rem;
      text-align: center;
    }

    .nav-links.active {
      display: flex;
    }
    
    .hero {
      padding: 0 5%;
    }

    .hero h1 {
      font-size: 2rem;
    }

    .hero p {
      font-size: 1rem;
    }

    .services,
    .team,
    .contact {
      padding: 3rem 5%;
    }

    .services-grid,
    .team-grid {
      grid-template-columns: 1fr;
      gap: 1.5rem;
    }

    .service-card,
    .team-member {
      padding: 1.5rem;
    }

    .team-member .avatar {
      width: 120px;
      height: 120px;
    }

    .section-title {
      font-size: 1.8rem;
      margin-bottom: 2rem;
    }
  }

  @media (max-width: 480px) {
    .hero h1 {
      font-size: 1.8rem;
    }

    .cta-button {
      padding: 0.8rem 1.5rem;
      font-size: 0.9rem;
    }

    .service-card,
    .team-member {
      padding: 1rem;
    }
  }
</style>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
</head>
<body>
  <nav>
    <div class="logo">UNLu Consulting Group</div>
    <button class="mobile-menu-btn">
      <i class="fas fa-bars"></i>
    </button>
    <div class="nav-links">
      <a href="#inicio">Inicio</a>
      <a href="#servicios">Servicios</a>
      <a href="#nosotros">Nosotros</a>
      <a href="#contacto">Contacto</a>
    </div>
  </nav>

  <header class="header" id="inicio">
    <div class="hero">
      <div>
        <h2>Transformamos tu negocio para el futuro</h2>
        <p>Soluciones estratégicas personalizadas para impulsar el crecimiento de tu empresa</p>
        <a href="#contacto" class="cta-button">Consulta Gratuita</a>
      </div>
    </div>
  </header>

  <section class="services" id="servicios">
    <h3 class="section-title">Nuestros Servicios</h3>
    <div class="services-grid">
      <div class="service-card">
        <i class="fas fa-chart-line service-icon"></i>
        <h3>Estrategia Empresarial</h3>
        <p>Desarrollamos estrategias personalizadas para maximizar el potencial de tu negocio.</p>
      </div>
      <div class="service-card">
        <i class="fas fa-users service-icon"></i>
        <h3>Gestión del Cambio</h3>
        <p>Facilitamos la transformación organizacional para adaptarse a nuevos desafíos.</p>
      </div>
      <div class="service-card">
        <i class="fas fa-globe service-icon"></i>
        <h4>Expansión Internacional</h4>
        <p>Te ayudamos a expandir tu negocio a nuevos mercados globales.</p>
      </div>
    </div>
  </section>

  <section class="team" id="nosotros">
    <h3 class="section-title">Nuestro Equipo</h3>
    <div class="team-grid">
      <div class="team-member">
        <div class="avatar">
          <i class="fas fa-user"></i>
        </div>
        <h3>Lic. Esteban Juan</h3>
        <p>Consultor Senior</p>
      </div>
      <div class="team-member">
        <div class="avatar">
          <i class="fas fa-user"></i>
        </div>
        <h3>Lic. Lischetti Pablo</h3>
        <p>Consultor Senior</p>
      </div>
      <div class="team-member">
        <div class="avatar">
          <i class="fas fa-user"></i>
        </div>
        <h3>Lic. Russo Sonia</h3>
        <p>Consultora Senior</p>
      </div>
      <div class="team-member">
        <div class="avatar">
          <i class="fas fa-user"></i>
        </div>
        <h3>Lic. Torres Natalia</h3>
        <p>Consultora Senior</p>
      </div>
    </div>
  </section>

  <section class="contact" id="contacto">
    <h2 class="section-title">Contáctanos</h2>
    <form class="contact-form" id="contactForm">
      <div class="form-group">
        <input type="text" placeholder="Nombre" required>
      </div>
      <div class="form-group">
        <input type="email" placeholder="Email" required>
      </div>
      <div class="form-group">
        <textarea placeholder="Mensaje" rows="5" required></textarea>
      </div>
      <button type="submit" class="submit-btn">Enviar Mensaje</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2024 UNLu Consulting Group. Todos los derechos reservados.</p>
  </footer>

  <script>
    const mobileMenuBtn = document.querySelector('.mobile-menu-btn');
    const navLinks = document.querySelector('.nav-links');

    mobileMenuBtn.addEventListener('click', () => {
      navLinks.classList.toggle('active');
    });

    document.getElementById('contactForm').addEventListener('submit', function(e) {
      e.preventDefault();
      alert('¡Gracias por tu mensaje! Nos pondremos en contacto contigo pronto.');
      this.reset();
    });

    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href')).scrollIntoView({
          behavior: 'smooth'
        });
        if (navLinks.classList.contains('active')) {
          navLinks.classList.remove('active');
        }
      });
    });
  </script>
</body></html>
