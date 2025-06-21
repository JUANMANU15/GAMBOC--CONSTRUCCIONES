# GAMBOC -CONSTRUCCIONES
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Gamboc Construcciones | Calidad y Profesionalismo</title>
  <meta name="description" content="Empresa especializada en construcción, remodelación y mantenimiento con más de 20 años de experiencia">
  <link href="https://fonts.googleapis.com/css2?family=Rubik:wght@300;400;500;600;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    :root {
      --primario: #000000;
      --secundario: #ffcc00;
      --claro: #fff8dc;
      --blanco: #ffffff;
      --gris: #f8f9fa;
      --sombra: 0 4px 12px rgba(0,0,0,0.1);
    }
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Rubik', sans-serif;
      background-color: var(--gris);
      color: var(--primario);
      line-height: 1.6;
      scroll-behavior: smooth;
    }
    header {
      background: linear-gradient(to right, var(--primario), #333);
      color: var(--secundario);
      padding: 1rem 1.5rem;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: var(--sombra);
    }
    .header-container {
      max-width: 1200px;
      margin: 0 auto;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    header h1 {
      font-size: 2.2rem;
      margin-bottom: 0.5rem;
      font-weight: 700;
    }
    nav {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1rem;
      margin-top: 0.5rem;
    }
    nav a {
      color: var(--secundario);
      text-decoration: none;
      font-weight: 500;
      padding: 0.5rem 1rem;
      border-radius: 4px;
      transition: all 0.3s ease;
      white-space: nowrap;
    }
    nav a:hover, nav a:focus {
      background-color: rgba(255, 204, 0, 0.2);
      transform: translateY(-2px);
    }
    section {
      padding: 4rem 1.5rem;
      max-width: 1200px;
      margin: auto;
    }
    h2 {
      color: var(--primario);
      margin-bottom: 1.5rem;
      font-size: 2rem;
      border-left: 5px solid var(--secundario);
      padding-left: 1rem;
      position: relative;
    }
    h2::after {
      content: '';
      position: absolute;
      bottom: -8px;
      left: 0;
      width: 50px;
      height: 3px;
      background-color: var(--secundario);
    }
    p {
      margin-bottom: 1rem;
      font-size: 1.1rem;
    }
    ul {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 1.5rem;
      list-style: none;
      padding: 0;
    }
    li {
      background-color: var(--blanco);
      padding: 1.5rem;
      border-left: 4px solid var(--secundario);
      border-radius: 8px;
      box-shadow: var(--sombra);
      transition: transform 0.3s ease;
    }
    li:hover {
      transform: translateY(-5px);
    }
    .contacto p {
      margin: 1rem 0;
      display: flex;
      align-items: center;
      gap: 0.8rem;
    }
    .contacto a {
      color: var(--primario);
      text-decoration: none;
      transition: color 0.3s ease;
    }
    .contacto a:hover {
      color: var(--secundario);
      text-decoration: underline;
    }
    footer {
      background-color: var(--primario);
      color: var(--secundario);
      text-align: center;
      padding: 2rem 1rem;
      margin-top: 2rem;
    }
    .galeria {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 1.5rem;
    }
    .galeria img {
      width: 100%;
      height: 220px;
      object-fit: cover;
      border-radius: 8px;
      box-shadow: var(--sombra);
      transition: transform 0.3s ease;
      cursor: pointer;
    }
    .galeria img:hover {
      transform: scale(1.03);
    }
    .hero {
      background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('imagenes/hero.jpg') center/cover no-repeat;
      color: var(--blanco);
      text-align: center;
      padding: 6rem 1.5rem;
      margin-bottom: 2rem;
    }
    .hero h2 {
      color: var(--secundario);
      border-left: none;
      font-size: 2.5rem;
      margin-bottom: 1.5rem;
    }
    .hero p {
      max-width: 800px;
      margin: 0 auto 2rem;
      font-size: 1.2rem;
    }
    .btn {
      display: inline-block;
      background-color: var(--secundario);
      color: var(--primario);
      padding: 0.8rem 1.8rem;
      border-radius: 4px;
      text-decoration: none;
      font-weight: 600;
      transition: all 0.3s ease;
      border: 2px solid var(--secundario);
    }
    .btn:hover {
      background-color: transparent;
      color: var(--secundario);
      transform: translateY(-3px);
    }
    .whatsapp-btn {
      position: fixed;
      bottom: 2rem;
      right: 2rem;
      background-color: #25D366;
      color: white;
      width: 60px;
      height: 60px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 2rem;
      box-shadow: 0 4px 12px rgba(0,0,0,0.2);
      z-index: 999;
      transition: all 0.3s ease;
      text-decoration: none;
    }
    .whatsapp-btn:hover {
      transform: scale(1.1) translateY(-5px);
      box-shadow: 0 6px 16px rgba(0,0,0,0.3);
    }
    .valor-item {
      display: flex;
      align-items: center;
      gap: 1rem;
      margin-bottom: 1rem;
    }
    .valor-icon {
      color: var(--secundario);
      font-size: 1.5rem;
    }
    .testimonios {
      background-color: var(--blanco);
      padding: 3rem;
      border-radius: 8px;
      box-shadow: var(--sombra);
      margin-top: 2rem;
    }
    @media (max-width: 768px) {
      section {
        padding: 3rem 1rem;
      }
      h2 {
        font-size: 1.6rem;
      }
      .hero {
        padding: 4rem 1rem;
      }
      .hero h2 {
        font-size: 2rem;
      }
    }
  </style>
</head>
<body>
  <header>
    <div class="header-container">
      <h1>Gamboc Construcciones</h1>
      <nav>
        <a href="#quienes"><i class="fas fa-building"></i> ¿Quiénes Somos?</a>
        <a href="#valores"><i class="fas fa-star"></i> Valores</a>
        <a href="#servicios"><i class="fas fa-tools"></i> Servicios</a>
        <a href="#galeria"><i class="fas fa-images"></i> Galería</a>
        <a href="#contacto"><i class="fas fa-envelope"></i> Contacto</a>
      </nav>
    </div>
  </header>

  <section class="hero">
    <h2>Construyendo tus sueños con calidad y profesionalismo</h2>
    <p>Más de 20 años de experiencia en construcción, remodelación y mantenimiento de espacios residenciales y comerciales</p>
    <a href="#contacto" class="btn">Contáctanos</a>
  </section>

  <section id="quienes">
    <h2>¿Quiénes Somos?</h2>
    <p>Somos una empresa comprometida con la calidad de nuestros servicios, asegurando resultados efectivos en cada proyecto. En Gamboc Construcciones tenemos el propósito de "construir la historia" de cada uno de nuestros clientes a través del cuidado y mantenimiento de sus espacios.</p>
    <p>Con más de 20 años de experiencia como empresa familiar en el sector de la construcción, nos rigen principios sólidos y un fuerte compromiso con nuestro trabajo. Nuestro objetivo principal es brindar garantía y calidad a las necesidades de nuestros clientes.</p>
    
    <div class="testimonios">
      <h3>Lo que dicen nuestros clientes</h3>
      <p><i>"Excelente trabajo en la remodelación de mi cocina, cumplieron con todos los plazos y el resultado superó mis expectativas."</i> - María González</p>
      <p><i>"Profesionales y puntuales. Recomiendo ampliamente sus servicios de construcción."</i> - Juan Pérez</p>
    </div>
  </section>

  <section id="valores">
    <h2>Nuestra Filosofía</h2>
    
    <div class="valor-item">
      <div class="valor-icon"><i class="fas fa-bullseye"></i></div>
      <div>
        <h3>Misión</h3>
        <p>Construir y remodelar espacios para que nuestros clientes tengan una alta calidad de vida, mejorando e innovando el lugar donde trabajan, descansan o se recrean, con técnicas vanguardistas sin perder las estructuras tradicionales, recuperando la historia de cada hogar.</p>
      </div>
    </div>
    
    <div class="valor-item">
      <div class="valor-icon"><i class="fas fa-eye"></i></div>
      <div>
        <h3>Visión</h3>
        <p>Ser una empresa reconocida por su capacidad de crecimiento, así como la garantía, actualización y eficacia de sus servicios.</p>
      </div>
    </div>
    
    <h2>Nuestros Valores</h2>
    <ul>
      <li><i class="fas fa-handshake valor-icon"></i> Compromiso</li>
      <li><i class="fas fa-user-tie valor-icon"></i> Profesionalismo</li>
      <li><i class="fas fa-balance-scale valor-icon"></i> Honestidad</li>
      <li><i class="fas fa-heart valor-icon"></i> Dedicación</li>
      <li><i class="fas fa-gavel valor-icon"></i> Trato justo</li>
      <li><i class="fas fa-users valor-icon"></i> Trabajo en equipo</li>
      <li><i class="fas fa-clock valor-icon"></i> Puntualidad</li>
    </ul>
  </section>

  <section id="politicas">
    <h2>Políticas de Calidad</h2>
    <p>Nuestras políticas se basan en brindar un servicio de calidad que cumpla con las expectativas del cliente, en un marco de respeto, cumplimiento normativo, mejora continua y seguridad para nuestros colaboradores.</p>
    <p>Nos aseguramos de:</p>
    <ul>
      <li><i class="fas fa-check-circle"></i> Cumplir con los tiempos establecidos en cada proyecto</li>
      <li><i class="fas fa-check-circle"></i> Utilizar materiales de calidad y técnicas adecuadas</li>
      <li><i class="fas fa-check-circle"></i> Ofrecer atención personalizada y seguimiento puntual</li>
      <li><i class="fas fa-check-circle"></i> Proteger la integridad de nuestro personal y del cliente</li>
      <li><i class="fas fa-check-circle"></i> Fomentar una cultura de trabajo ordenada, limpia y eficiente</li>
    </ul>
  </section>

  <section id="servicios">
    <h2>Nuestros Servicios</h2>
    <p>Ofrecemos soluciones integrales para todas tus necesidades de construcción y remodelación:</p>
    <ul>
      <li><i class="fas fa-bolt"></i> Remodelación e instalación eléctrica</li>
      <li><i class="fas fa-tint"></i> Drenaje y alimentación de agua</li>
      <li><i class="fas fa-border-style"></i> Instalación de muros de tablaroca</li>
      <li><i class="fas fa-square"></i> Pisos y azulejos</li>
      <li><i class="fas fa-toolbox"></i> Proyectos de mantenimiento menor</li>
      <li><i class="fas fa-mountain"></i> Acabados de concreto y piedra</li>
      <li><i class="fas fa-hammer"></i> Albañilería en general</li>
      <li><i class="fas fa-plug"></i> Electricidad y fontanería</li>
      <li><i class="fas fa-layer-group"></i> Plafones, enjarres y techos</li>
      <li><i class="fas fa-lightbulb"></i> Instalación de lámparas</li>
      <li><i class="fas fa-toilet"></i> Drenaje para inodoro y lavabo</li>
      <li><i class="fas fa-utensils"></i> Colocación de estufa y campana</li>
      <li><i class="fas fa-road"></i> Loza y banquetas de concreto</li>
    </ul>
  </section>

  <section id="galeria">
    <h2>Galería de Proyectos</h2>
    <div class="galeria">
      <img src="imagenes/imagen_1_1.jpeg" alt="Instalación de tablaroca" loading="lazy">
      <img src="imagenes/imagen_1_3.png" alt="Acabado de muros" loading="lazy">
      <img src="imagenes/imagen_2_5.jpeg" alt="Piso y azulejo en cocina" loading="lazy">
      <img src="imagenes/imagen_3_3.jpeg" alt="Drenaje y fontanería" loading="lazy">
      <img src="imagenes/imagen_4_1.jpeg" alt="Colocación de estufa eléctrica" loading="lazy">
      <img src="imagenes/imagen_5_4.jpeg" alt="Loza de concreto con tubería de luz" loading="lazy">
    </div>
  </section>

  <section id="contacto" class="contacto">
    <h2>Contacto</h2>
    <p><i class="fas fa-user-tie"></i> <strong>Nombre:</strong> ING. ROBERTO GÁMEZ BOCANEGRA</p>
    <p><i class="fab fa-whatsapp"></i> <strong>WhatsApp:</strong> <a href="https://wa.me/524733200921">473 320 0921</a></p>
    <p><i class="fab fa-facebook"></i> <strong>Facebook:</strong> <a href="https://facebook.com/ConstructoraGamboc" target="_blank">Constructora Gamboc</a></p>
    <p><i class="fas fa-envelope"></i> <strong>Email:</strong> <a href="mailto:gamboconstrucciones@gmail.com">gamboconstrucciones@gmail.com</a></p>
    <p><i class="fas fa-map-marker-alt"></i> <strong>Dirección:</strong> Carretera a las momias, Guanajuato, Gto. México</p>
  </section>

  <footer>
    <p>&copy; 2025 Gamboc Construcciones. Todos los derechos reservados.</p>
    <div style="margin-top: 1rem;">
      <a href="#" style="color: var(--secundario); margin: 0 0.5rem;"><i class="fab fa-facebook-f"></i></a>
      <a href="#" style="color: var(--secundario); margin: 0 0.5rem;"><i class="fab fa-instagram"></i></a>
      <a href="#" style="color: var(--secundario); margin: 0 0.5rem;"><i class="fab fa-linkedin-in"></i></a>
    </div>
  </footer>

  <a href="https://wa.me/524733200921" class="whatsapp-btn" aria-label="Contactar por WhatsApp">
    <i class="fab fa-whatsapp"></i>
  </a>

  <script>
    // Efecto suave al hacer clic en los enlaces del menú
    document.querySelectorAll('nav a').forEach(anchor => {
      anchor.addEventListener('click', function(e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href')).scrollIntoView({
          behavior: 'smooth'
        });
      });
    });

    // Animación para los elementos al hacer scroll
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.style.opacity = 1;
          entry.target.style.transform = 'translateY(0)';
        }
      });
    }, { threshold: 0.1 });

    document.querySelectorAll('section, .galeria img').forEach(section => {
      section.style.opacity = 0;
      section.style.transform = 'translateY(20px)';
      section.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
      observer.observe(section);
    });
  </script>
</body>
</html>
