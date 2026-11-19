<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Partido Macorina y El Peña | Criadero de Gallos Finos</title>
    <!-- Fuentes de Google para darle un toque clásico y moderno a la vez -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@600;800&family=Montserrat:wght@300;400;600&display=swap" rel="stylesheet">
    
    <style>
        /* --- VARIABLES DE COLOR Y ESTILO --- */
        :root {
            --bg-dark: #12100e;       /* Negro carbón / madera oscura */
            --bg-card: #1d1916;       /* Marrón muy oscuro para tarjetas */
            --gold: #d4af37;          /* Dorado clásico */
            --gold-hover: #f3ce5b;    /* Dorado brillante */
            --crimson: #8b1e1e;       /* Rojo sangre / cresta */
            --text-light: #f5f5f5;    /* Blanco hueso */
            --text-muted: #a89f91;    /* Gris cálido */
        }

        /* --- RESET BÁSICO --- */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background-color: var(--bg-dark);
            color: var(--text-light);
            line-height: 1.6;
        }

        h1, h2, h3, .logo {
            font-family: 'Cinzel', serif;
            letter-spacing: 1px;
        }

        /* --- BARRA DE NAVEGACIÓN --- */
        header {
            background-color: rgba(18, 16, 14, 0.95);
            border-bottom: 2px solid var(--gold);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            padding: 15px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 800;
            color: var(--gold);
            text-decoration: none;
            text-transform: uppercase;
        }

        .logo span {
            color: var(--text-light);
            font-size: 1.1rem;
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 25px;
        }

        nav a {
            color: var(--text-light);
            text-decoration: none;
            font-weight: 600;
            font-size: 0.9rem;
            text-transform: uppercase;
            transition: color 0.3s;
        }

        nav a:hover {
            color: var(--gold);
        }

        /* --- SECCIÓN PRINCIPAL (HERO) --- */
        .hero {
            height: 100vh;
            background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(18, 16, 14, 0.95)), 
                        url('https://images.unsplash.com/photo-1548550023-2bdb3c5beed7?auto=format&fit=crop&w=1920&q=80') center/cover no-repeat;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 0 20px;
            margin-top: 60px;
        }

        .hero-subtitle {
            color: var(--gold);
            font-size: 1.1rem;
            text-transform: uppercase;
            letter-spacing: 4px;
            margin-bottom: 10px;
            font-weight: 600;
        }

        .hero h1 {
            font-size: 3.8rem;
            color: var(--text-light);
            margin-bottom: 20px;
            text-shadow: 2px 4px 10px rgba(0,0,0,0.8);
        }

        .hero p {
            max-width: 650px;
            color: var(--text-muted);
            font-size: 1.1rem;
            margin-bottom: 35px;
        }

        .btn {
            display: inline-block;
            padding: 14px 32px;
            background-color: var(--crimson);
            color: var(--text-light);
            text-decoration: none;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 1.5px;
            border: 1px solid var(--gold);
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .btn:hover {
            background-color: var(--gold);
            color: var(--bg-dark);
        }

        /* --- ESTILOS GENERALES DE SECCIÓN --- */
        section {
            padding: 80px 8%;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }

        .section-title h2 {
            font-size: 2.5rem;
            color: var(--gold);
            margin-bottom: 10px;
        }

        .section-title .divider {
            width: 80px;
            height: 3px;
            background-color: var(--crimson);
            margin: 0 auto;
        }
        /* --- NOSOTROS --- */
        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            align-items: center;
        }

        .about-text h3 {
            font-size: 1.8rem;
            margin-bottom: 15px;
            color: var(--text-light);
        }

        .about-text p {
            color: var(--text-muted);
            margin-bottom: 15px;
        }

        .about-stats {
            display: flex;
            gap: 30px;
            margin-top: 25px;
            border-top: 1px solid #332c26;
            padding-top: 20px;
        }

        .stat h4 {
            font-family: 'Cinzel', serif;
            font-size: 2rem;
            color: var(--gold);
        }

        .stat span {
            font-size: 0.85rem;
            color: var(--text-muted);
            text-transform: uppercase;
        }

        .about-img {
            border: 2px solid var(--gold);
            padding: 10px;
            background-color: var(--bg-card);
        }

        .about-img img {
            width: 100%;
            height: auto;
            display: block;
            filter: contrast(1.1);
        }

        /* --- LÍNEAS DE SANGRE (TARJETAS) --- */
        .bloodlines {
            background-color: #161311;
        }

        .cards-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
        }

        .card {
            background-color: var(--bg-card);
            border: 1px solid #332c26;
            transition: transform 0.3s, border-color 0.3s;
            overflow: hidden;
        }

        .card:hover {
            transform: translateY(-8px);
            border-color: var(--gold);
        }

        .card-img {
            height: 220px;
            background-color: #2a241f;
            overflow: hidden;
            position: relative;
        }

        .card-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s;
        }

        .card:hover .card-img img {
            transform: scale(1.08);
        }

        .tag {
            position: absolute;
            top: 12px;
            right: 12px;
            background-color: var(--crimson);
            color: var(--text-light);
            padding: 4px 10px;
            font-size: 0.75rem;
            font-weight: 600;
            text-transform: uppercase;
            border: 1px solid var(--gold);
        }

        .card-content {
            padding: 25px;
        }

        .card-content h3 {
            color: var(--gold);
            font-size: 1.4rem;
            margin-bottom: 10px;
        }

        .card-content p {
            color: var(--text-muted);
            font-size: 0.95rem;
            margin-bottom: 15px;
        }

        .specs {
            list-style: none;
            font-size: 0.85rem;
            color: var(--text-light);
            border-top: 1px solid #332c26;
            padding-top: 12px;
        }

        .specs li {
            margin-bottom: 5px;
        }

        .specs strong {
            color: var(--gold);
        }

        /* --- CONTACTO --- */
        .contact-container {
            max-width: 700px;
            margin: 0 auto;
            background-color: var(--bg-card);
            padding: 40px;
            border: 1px solid var(--gold);
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            color: var(--gold);
            font-size: 0.9rem;
            text-transform: uppercase;
        }

        .form-group input,
        .form-group select,
        .form-group textarea {
            width: 100%;
            padding: 12px;
            background-color: var(--bg-dark);
            border: 1px solid #3d352e;
            color: var(--text-light);
            font-family: 'Montserrat', sans-serif;
        }

        .form-group input:focus,
        .form-group select:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: var(--gold);
        }

        .contact-container .btn {
            width: 100%;
            text-align: center;
        }

        /* --- FOOTER --- */
        footer {
            background-color: #0b0a09;
            text-align: center;
            padding: 30px 20px;
            border-top: 1px solid #2b2520;
            color: var(--text-muted);
            font-size: 0.9rem;
        }

        footer strong {
            color: var(--gold);
        }

        /* --- RESPONSIVE (MÓVILES) --- */
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                gap: 10px;
            }
            .hero h1 {
                font-size: 2.5rem;
            }
            .about-grid {
                grid-template-columns: 1fr;
            }
            nav ul {
                gap: 15px;
                font-size: 0.8rem;
            }
        }
    </style>
</head>
<body>

    <!-- ENCABEZADO Y NAVEGACIÓN -->
    <header>
        <a href="#" class="logo">Partido <span>Macorina y El Peña</span></a>
        <nav>
            <ul>
                <li><a href="#inicio">Inicio</a></li>
                <li><a href="#nosotros">El Criadero</a></li>
                <li><a href="#lineas">Líneas de Sangre</a></li>
                <li><a href="#contacto">Contacto</a></li>
            </ul>
        </nav>
    </header>

    <!-- PORTADA PRINCIPAL -->
    <section id="inicio" class="hero">
        <span class="hero-subtitle">Criadero de Gallos Finos</span>
        <h1>Partido Macorina y El Peña</h1>
        <p>Selección genética de alto rendimiento, casta probada en los mejores palenques y crianza bajo estrictos estándares de salud y acondicionamiento.</p>
        <a href="#lineas" class="btn">Conocer Nuestras Líneas</a>
    </section>

    <!-- SECCIÓN EL CRIADERO -->
    <section id="nosotros">
        <div class="section-title">
            <h2>Tradición y Casta</h2>
            <div class="divider"></div>
        </div>
        <div class="about-grid">
            <div class="about-text">
                <h3>Pasión por la Gallística</h3>
                <p>En <strong>Partido Macorina y El Peña</strong> nos dedicamos a la crianza, selección y cuido de aves de combate de la más alta calidad. Nuestro compromiso radica en mantener sangres
                 limpias y realizar cruzas estratégicas que garanticen inteligencia, corte y resistencia.</p>
                <p>Cada ejemplar cuenta con registro genealógico, alimentación balanceada desde el nacimiento y amplios voladeros para un desarrollo muscular óptimo.</p>
                
                <div class="about-stats">
                    <div class="stat">
                        <h4>100%</h4>
                        <span>Sangre Probada</span>
                    </div>
                    <div class="stat">
                        <h4>+15</h4>
                        <span>Años de Experiencia</span>
                    </div>
                    <div class="stat">
                        <h4>Top</h4>
                        <span>Genética Importada</span>
                    </div>
                </div>    
            </div>
            <div class="about-img">
                <!-- Imagen referencial de gallo -->
                <img src="https://images.unsplash.com/photo-1569396116180-210c182bedb8?auto=format&fit=crop&w=800&q=80" alt="Ejemplar del Criadero"
            </div>
        </div>
    </section>

    <!-- SECCIÓN LÍNEAS DE SANGRE -->
    <section id="lineas" class="bloodlines">
        <div class="section-title">
            <h2>Nuestras Líneas de Sangre</h2>
            <div class="divider"></div>
        </div>
        
        <div class="cards-grid">
            <!-- Tarjeta 1 -->
            <div class="card">
                <div class="card-img">
                    <span class="tag">Semental Base</span>
 <img src="https://images.unsplash.com/photo-1612170153139-6f881ff067e0?auto=format&fit=crop&w=600&q=80" alt="Línea Kelso">
                </div>
                <div class="card-content">
                    <h3>Yellow Leg Hatch</h3>
                    <p>La base de la resistencia y el coraje. Aves fuertes que no ceden terreno y definen en el suelo o aire.</p>
                    <ul class="specs">
                        <li><strong>Pluma:</strong> Retinto / Colorado</li>
                        <li><strong>Estilo:</strong> Fuerza y resistencia</li>
                        <li><strong>Disponibilidad:</strong> Sobre pedido</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
    <!-- SECCIÓN LÍNEAS DE SANGRE -->
    <section id="lineas" class="bloodlines">
        <div class="section-title">
            <h2>Nuestras Líneas de Sangre</h2>
            <div class="divider"></div>
        </div>
        
        <div class="cards-grid">
            <!-- Tarjeta 1 -->
            <div class="card">
                <div class="card-img">
                    <span class="tag">Semental Base</span>
 <img src="https://images.unsplash.com/photo-1612170153139-6f881ff067e0?auto=format&fit=crop&w=600&q=80" alt="Línea Kelso">
                </div>
                <div class="card-content">
                    <h3>Yellow Leg Hatch</h3>
                    <p>La base de la resistencia y el coraje. Aves fuertes que no ceden terreno y definen en el suelo o aire.</p>
                    <ul class="specs">
                        <li><strong>Pluma:</strong> Retinto / Colorado</li>
                        <li><strong>Estilo:</strong> Fuerza y resistencia</li>
                        <li><strong>Disponibilidad:</strong> Sobre pedido</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
    <!-- SECCIÓN LÍNEAS DE SANGRE -->
    <section id="lineas" class="bloodlines">
        <div class="section-title">
            <h2>Nuestras Líneas de Sangre</h2>
            <div class="divider"></div>
        </div>
        
        <div class="cards-grid">
            <!-- Tarjeta 1 -->
            <div class="card">
                <div class="card-img">
                    <span class="tag">Semental Base</span>
                </div>
                <div class="card-content">
                    <h3>Yellow Leg Hatch</h3>
                    <p>La base de la resistencia y el coraje. Aves fuertes que no ceden terreno y definen en el suelo o aire.</p>
                    <ul class="specs">
                        <li><strong>Pluma:</strong> Retinto / Colorado</li>
                        <li><strong>Estilo:</strong> Fuerza y resistencia</li>
                        <li><strong>Disponibilidad:</strong> Sobre pedido</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- SECCIÓN CONTACTO -->
    <section id="contacto">
        <div class="section-title">
            <h2>Contacto y Ventas</h2>
            <div class="divider"></div>
        </div>

        <div class="contact-container">
            <form action="#" method="POST">
                <div class="form-group">
                    <label for="nombre">Nombre Completo</label>
                    <input type="text" id="nombre" name="nombre" placeholder="Ej. Juan Pérez" required>
                </div>

                <div class="form-group">
                    <label for="telefono">Teléfono / WhatsApp</label>
                    <input type="tel" id="telefono" name="telefono" placeholder="Ej. 844 123 4567" required>
                </div>

                <div class="form-group">
                    <label for="interes">Motivo de Contacto</label>
                    <select id="interes" name="interes">
                        <option value="pies-de-cria">Adquisición de Pies de Cría</option>
                        <option value="pollos">Lote de Pollos</option>
                        <option value="compromisos">Invitación a Compromiso / Torneo</option>
                        <option value="otro">Información General</option>
                    </select>
                </div>

                <div class="form-group">
                    <label for="mensaje">Mensaje</label>
                    <textarea id="mensaje" name="mensaje" rows="4" placeholder="Escribe los detalles de lo que buscas..."></textarea>
                </div>

                <button type="submit" class="btn">Enviar Mensaje</button>
            </form>
        </div>
    </section>

    <!-- PIE DE PÁGINA -->
    <footer>
        <p>&copy; 2026 <strong>Partido Macorina y El Peña</strong> - Criadero de Gallos Finos. Todos los derechos reservados.</p>
    </footer>

</body>
</html>
