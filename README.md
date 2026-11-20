
<html lang="es" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Partido Macorina y El Peña | Criadero de Gallos Finos</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@600;700;800&family=Playfair+Display:ital,wght@0,500;0,700;1,400&family=Plus+Jakarta+Sans:wght@400;500;600&display=swap" rel="stylesheet">
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        crimson: {
                            DEFAULT: '#6b1218',
                            dark: '#42090d',
                            light: '#8f1b23',
                        },
                        gold: {
                            DEFAULT: '#c59b27',
                            light: '#e0bc53',
                            dark: '#967213',
                        },
                        earth: {
                            dark: '#14110f',
                            card: '#1f1a17',
                            border: '#362d27',
                            sand: '#ede6db',
                            muted: '#a89f94'
                        }
                    },
                    fontFamily: {
                        display: ['Cinzel', 'serif'],
                        serif: ['Playfair Display', 'serif'],
                        sans: ['Plus Jakarta Sans', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <style>
        .bg-hero-pattern {
            background-color: #14110f;
            background-image: 
                radial-gradient(circle at 50% 35%, rgba(107, 18, 24, 0.45) 0%, rgba(20, 17, 15, 0.96) 75%),
                url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23c59b27' fill-opacity='0.05'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
        }
        .gold-divider {
            height: 2px;
            background: linear-gradient(90deg, transparent, #c59b27, transparent);
        }
    </style>
</head>
<body class="bg-earth-dark text-earth-sand font-sans antialiased selection:bg-crimson selection:text-gold-light">

    <!-- Navegación -->
    <header class="fixed top-0 w-full z-50 bg-earth-dark/90 backdrop-blur-md border-b border-earth-border">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <!-- Logo / Nombre -->
                <a href="#inicio" class="flex items-center space-x-3 group">
                    <div class="w-10 h-10 rounded-full bg-crimson border border-gold flex items-center justify-center shadow-lg group-hover:scale-105 transition-transform">
                        <i data-lucide="award" class="w-5 h-5 text-gold-light"></i>
                    </div>
                    <div>
                        <span class="font-display font-bold text-lg tracking-wider text-gold-light block leading-none">MACORINA Y EL PEÑA</span>
                        <span class="text-[11px] uppercase tracking-[0.2em] text-earth-muted">Criadero de Gallos Finos</span>
                    </div>
                </a>

                <!-- Enlaces Desktop -->
                <nav class="hidden md:flex space-x-8 text-sm font-medium tracking-wide">
                    <a href="#historia" class="text-earth-sand hover:text-gold-light transition-colors">Tradición</a>
                    <a href="#lineas" class="text-earth-sand hover:text-gold-light transition-colors">Líneas Genéticas</a>
                    <a href="#instalaciones" class="text-earth-sand hover:text-gold-light transition-colors">Crianza</a>
                    <a href="#ubicacion" class="text-earth-sand hover:text-gold-light transition-colors">Ubicación y Contacto</a>
                </nav>

                <!-- Botón Directo WhatsApp -->
                <div class="hidden sm:block">
                    <a href="https://wa.me/525666401617" target="_blank" rel="noopener noreferrer" 
                       class="inline-flex items-center gap-2 px-4 py-2 rounded border border-gold text-gold-light hover:bg-gold hover:text-earth-dark font-semibold text-xs uppercase tracking-wider transition-all">
                        <i data-lucide="phone-call" class="w-3.5 h-3.5"></i>
                        Trato Directo
                    </a>
                </div>
            </div>
        </div>
    </header>

    <!-- Sección Principal (Hero) -->
    <section id="inicio" class="relative pt-32 pb-24 md:pt-44 md:pb-36 bg-hero-pattern border-b border-earth-border overflow-hidden">
        <div class="max-w-5xl mx-auto px-4 sm:px-6 text-center relative z-10">
            <!-- Emblema Superior -->
            <div class="inline-flex items-center gap-2 px-4 py-1.5 rounded-full bg-earth-card border border-gold/40 text-gold-light text-xs uppercase tracking-[0.25em] mb-8">
                <i data-lucide="map-pin" class="w-3.5 h-3.5 text-gold"></i>
                Santa Isabel Ixtapan, Estado de México
            </div>

            <h1 class="font-display text-4xl sm:text-6xl md:text-7xl font-extrabold tracking-tight text-white mb-6 leading-tight">
                PARTIDO <br>
                <span class="text-transparent bg-clip-text bg-gradient-to-r from-gold-light via-gold to-gold-dark">
                    MACORINA Y EL PEÑA
                </span>
            </h1>

            <p class="font-serif italic text-xl sm:text-2xl text-earth-sand/90 max-w-2xl mx-auto mb-10">
                "Castas seleccionadas con rigor, crianza en libertad y respeto absoluto por la tradición gallística de México."
            </p>

            <div class="gold-divider max-w-md mx-auto mb-10"></div>

            <!-- Botones de Acción Directa (Sin formularios) -->
            <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
                <a href="#lineas" class="w-full sm:w-auto px-8 py-4 bg-crimson hover:bg-crimson-light text-white font-display font-bold tracking-widest text-sm uppercase rounded border border-gold/50 shadow-xl transition-all">
                    Conocer Nuestras Líneas
                </a>
                <a href="#ubicacion" class="w-full sm:w-auto px-8 py-4 bg-earth-card hover:bg-earth-border text-gold-light font-display font-bold tracking-widest text-sm uppercase rounded border border-earth-border transition-all">
                    Visitar el Criadero
                </a>
            </div>
        </div>
    </section>

    <!-- Historia y Tradición -->
    <section id="historia" class="py-20 md:py-28 bg-earth-dark">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                <!-- Columna Izquierda: Texto -->
                <div class="lg:col-span-7 space-y-6">
                    <span class="text-gold uppercase tracking-[0.25em] text-xs font-bold block">Nuestra Esencia</span>
                    <h2 class="font-display text-3xl sm:text-4xl font-bold text-white leading-snug">
                        Forjando Sangre de Campeones en Santa Isabel Ixtapan
                    </h2>
                    <div class="w-20 h-1 bg-crimson"></div>
                    <p class="text-earth-sand/85 leading-relaxed text-base sm:text-lg">
                        El <strong class="text-gold-light">Partido Macorina y El Peña</strong> nace de la pasión genuina y el compromiso con la crianza selectiva del gallo fino de combate. Arraigados en <strong>Santa Isabel Ixtapan</strong>, municipio de Atenco, hemos dedicado años a consolidar pies de cría que destacan por su inteligencia, corte, resistencia y ley.
                    </p>
                    <p class="text-earth-sand/85 leading-relaxed text-base sm:text-lg">
                        Cada ejemplar es criado bajo estrictos estándares de nutrición, sanidad y manejo en voladeros naturales, garantizando aves con plumaje impecable, estructura ósea sólida y un temperamento probado en los mejores palenques y derbies del país.
                    </p>

                    <!-- Pilares -->
                    <div class="grid grid-cols-3 gap-4 pt-4 border-t border-earth-border">
                        <div>
                            <span class="font-display text-2xl sm:text-3xl font-bold text-gold-light block">100%</span>
                            <span class="text-xs text-earth-muted uppercase tracking-wider">Sangre Seleccionada</span>
                        </div>
                        <div>
                            <span class="font-display text-2xl sm:text-3xl font-bold text-gold-light block">Crianza</span>
                            <span class="text-xs text-earth-muted uppercase tracking-wider">En Libertad y Sol</span>
                        </div>
                        <div>
                            <span class="font-display text-2xl sm:text-3xl font-bold text-gold-light block">Atenco</span>
                            <span class="text-xs text-earth-muted uppercase tracking-wider">Tradición Mexiquense</span>
                        </div>
                    </div>
                </div>

                <!-- Columna Derecha: Tarjeta Distintiva -->
                <div class="lg:col-span-5">
                    <div class="bg-earth-card border border-gold/30 rounded-lg p-8 shadow-2xl relative">
                        <div class="absolute -top-4 -right-4 w-12 h-12 bg-crimson border border-gold rounded-full flex items-center justify-center">
                            <i data-lucide="shield-check" class="w-6 h-6 text-gold-light"></i>
                        </div>
                        <h3 class="font-display text-xl font-bold text-gold-light mb-4 tracking-wide">Compromiso del Partido</h3>
                        <ul class="space-y-4 text-sm text-earth-sand/90">
                            <li class="flex items-start gap-3">
                                <i data-lucide="check-circle-2" class="w-5 h-5 text-gold shrink-0 mt-0.5"></i>
                                <span><strong>Registros Genealógicos:</strong> Control riguroso de cruzas, placas y anillos de nacimiento.</span>
                            </li>
                            <li class="flex items-start gap-3">
                                <i data-lucide="check-circle-2" class="w-5 h-5 text-gold shrink-0 mt-0.5"></i>
                                <span><strong>Medicina Preventiva:</strong> Calendarios completos de vacunación y desparasitación supervisados.</span>
                            </li>
                            <li class="flex items-start gap-3">
                                <i data-lucide="check-circle-2" class="w-5 h-5 text-gold shrink-0 mt-0.5"></i>
                                <span><strong>Selección Rigurosa:</strong> Solo los ejemplares que cumplen con fenotipo y casta pasan a reproducción.</span>
                            </li>
                            <li class="flex items-start gap-3">
                                <i data-lucide="check-circle-2" class="w-5 h-5 text-gold shrink-0 mt-0.5"></i>
                                <span><strong>Trato Serio y Directo:</strong> Atención personalizada en nuestro criadero previa cita.</span>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Líneas Genéticas -->
    <section id="lineas" class="py-20 md:py-28 bg-earth-card border-y border-earth-border">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-16">
                <span class="text-gold uppercase tracking-[0.25em] text-xs font-bold block mb-2">Pies de Cría</span>
                <h2 class="font-display text-3xl sm:text-4xl font-bold text-white mb-4">Nuestras Líneas Genéticas</h2>
                <p class="text-earth-muted text-sm sm:text-base">
                    Trabajamos sangres probadas que se complementan en velocidad, resistencia y capacidad de definición.
                </p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
                <!-- Línea 1 -->
                <div class="bg-earth-dark border border-earth-border hover:border-gold/60 rounded-lg p-6 transition-all group">
                    <div class="w-12 h-12 rounded bg-crimson/30 border border-crimson flex items-center justify-center mb-5 group-hover:bg-crimson transition-colors">
                        <i data-lucide="flame" class="w-6 h-6 text-gold-light"></i>
                    </div>
                    <h3 class="font-display text-xl font-bold text-gold-light mb-2">Kelso</h3>
                    <p class="text-xs uppercase tracking-widest text-earth-muted mb-3">Inteligencia y Rapidez</p>
                    <p class="text-sm text-earth-sand/80 leading-relaxed">
                        Aves de gran agilidad mental y desplazamiento lateral. Destacan por su capacidad para evitar el castigo y responder con precisión quirúrgica.
                    </p>
                </div>

                <!-- Línea 2 -->
                <div class="bg-earth-dark border border-earth-border hover:border-gold/60 rounded-lg p-6 transition-all group">
                    <div class="w-12 h-12 rounded bg-crimson/30 border border-crimson flex items-center justify-center mb-5 group-hover:bg-crimson transition-colors">
                        <i data-lucide="shield" class="w-6 h-6 text-gold-light"></i>
                    </div>
                    <h3 class="font-display text-xl font-bold text-gold-light mb-2">Hatch</h3>
                    <p class="text-xs uppercase tracking-widest text-earth-muted mb-3">Poder y Resistencia</p>
                    <p class="text-sm text-earth-sand/80 leading-relaxed">
                        Ejemplares de fuerte osamenta, golpe contundente y fondo inagotable. La base ideal para aportar fortaleza y corazón a nuestras cruzas.
                    </p>
                </div>

                <!-- Línea 3 -->
                <div class="bg-earth-dark border border-earth-border hover:border-gold/60 rounded-lg p-6 transition-all group">
                    <div class="w-12 h-12 rounded bg-crimson/30 border border-crimson flex items-center justify-center mb-5 group-hover:bg-crimson transition-colors">
                        <i data-lucide="zap" class="w-6 h-6 text-gold-light"></i>
                    </div>
                    <h3 class="font-display text-xl font-bold text-gold-light mb-2">Sweater</h3>
                    <p class="text-xs uppercase tracking-widest text-earth-muted mb-3">Explosividad y Corte</p>
                    <p class="text-sm text-earth-sand/80 leading-relaxed">
                        Gallos eléctricos, de gran vuelo y ofensiva constante. Reconocidos por su plumaje vistoso y su velocidad para definir desde el primer encuentro.
                    </p>
                </div>

                <!-- Línea 4 -->
                <div class="bg-earth-dark border border-earth-border hover:border-gold/60 rounded-lg p-6 transition-all group">
                    <div class="w-12 h-12 rounded bg-crimson/30 border border-crimson flex items-center justify-center mb-5 group-hover:bg-crimson transition-colors">
                        <i data-lucide="crown" class="w-6 h-6 text-gold-light"></i>
                    </div>
                    <h3 class="font-display text-xl font-bold text-gold-light mb-2">Asil / Orientales</h3>
                    <p class="text-xs uppercase tracking-widest text-earth-muted mb-3">Aplomo y Resistencia</p>
                    <p class="text-sm text-earth-sand/80 leading-relaxed">
                        Aportan musculatura densa, temple inquebrantable y resistencia superior para refrescar sangres y producir cuartos de milla altamente competitivos.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Instalaciones y Manejo -->
    <section id="instalaciones" class="py-20 md:py-28 bg-earth-dark">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-16">
                <span class="text-gold uppercase tracking-[0.25em] text-xs font-bold block mb-2">Infraestructura</span>
                <h2 class="font-display text-3xl sm:text-4xl font-bold text-white mb-4">Crianza y Desarrollo Integral</h2>
                <p class="text-earth-muted text-sm sm:text-base">
                    El entorno donde crece el gallo determina su rendimiento físico. Nuestras instalaciones en Santa Isabel Ixtapan están diseñadas para cada etapa de vida.
                </p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="border-l-2 border-gold pl-6 py-2">
                    <h3 class="font-display text-lg font-bold text-white mb-2">1. Lotes de Reproducción</h3>
                    <p class="text-sm text-earth-sand/80 leading-relaxed">
                        Corrales individuales amplios con sombra natural y control sanitario estricto para sementales y gallinas progenitoras.
                    </p>
                </div>
                <div class="border-l-2 border-gold pl-6 py-2">
                    <h3 class="font-display text-lg font-bold text-white mb-2">2. Sueltas y Voladeros</h3>
                    <p class="text-sm text-earth-sand/80 leading-relaxed">
                        Áreas arboladas donde los pollos desarrollan musculatura, capacidad pulmonar y reflejos naturales en libertad.
                    </p>
                </div>
                <div class="border-l-2 border-gold pl-6 py-2">
                    <h3 class="font-display text-lg font-bold text-white mb-2">3. Cuido y Acondicionamiento</h3>
                    <p class="text-sm text-earth-sand/80 leading-relaxed">
                        Rascaderos individuales ventilados y dieta balanceada a base de granos seleccionados, vitaminas y suplementación natural.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Ubicación y Contacto Directo (Sin Formularios) -->
    <footer id="ubicacion" class="bg-earth-card border-t border-gold/40 pt-16 pb-12">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-12 pb-12 border-b border-earth-border">
                
                <!-- Columna 1: Identidad -->
                <div>
                    <div class="flex items-center space-x-3 mb-4">
                        <div class="w-9 h-9 rounded-full bg-crimson border border-gold flex items-center justify-center">
                            <i data-lucide="award" class="w-4 h-4 text-gold-light"></i>
                        </div>
                        <span class="font-display font-bold text-lg text-gold-light tracking-wider">MACORINA Y EL PEÑA</span>
                    </div>
                    <p class="text-sm text-earth-muted leading-relaxed mb-4">
                        Criadero de gallos finos de combate. Dedicación, seriedad y respeto por la gallística mexicana.
                    </p>
                    <p class="text-xs text-gold/80 italic font-serif">
                        "La calidad de la sangre se demuestra en el ruedo."
                    </p>
                </div>

                <!-- Columna 2: Ubicación Exacta -->
                <div>
                    <h4 class="font-display text-sm font-bold uppercase tracking-widest text-white mb-4">Ubicación del Criadero</h4>
                    <ul class="space-y-3 text-sm text-earth-sand/85">
                        <li class="flex items-start gap-3">
                            <i data-lucide="map-pin" class="w-5 h-5 text-gold shrink-0 mt-0.5"></i>
                            <span>
                                <strong>Santa Isabel Ixtapan</strong><br>
                                Municipio de Atenco, Estado de México.<br>
                                <span class="text-xs text-earth-muted">Zona Texcoco / Atenco</span>
                            </span>
                        </li>
                        <li class="flex items-start gap-3">
                            <i data-lucide="clock" class="w-5 h-5 text-gold shrink-0 mt-0.5"></i>
                            <span>
                                <strong>Visitas al Criadero:</strong><br>
                                Lunes a Domingo (Únicamente previa cita).
                            </span>
                        </li>
                    </ul>
                </div>

                <!-- Columna 3: Canales Directos -->
                <div>
                    <h4 class="font-display text-sm font-bold uppercase tracking-widest text-white mb-4">Contacto Directo</h4>
                    <p class="text-xs text-earth-muted mb-4">
                        Para informes sobre disponibilidad de pies de cría, pollos o visitas, comuníquese directamente por vía telefónica o WhatsApp:
                    </p>
                    <div class="space-y-3">
                        <a href="https://wa.me/5666401617" target="_blank" rel="noopener noreferrer" 
                           class="flex items-center justify-center gap-2 w-full py-3 px-4 bg-[#1e5c3a] hover:bg-[#257348] text-white font-semibold text-sm rounded transition-colors">
                            <i data-lucide="message-circle" class="w-4 h-4"></i>
                            Enviar WhatsApp Directo
                        </a>
                        <a href="tel:+525666401617" 
                           class="flex items-center justify-center gap-2 w-full py-3 px-4 bg-earth-dark hover:bg-earth-border border border-gold/40 text-gold-light font-semibold text-sm rounded transition-colors">
                            <i data-lucide="phone" class="w-4 h-4"></i>
                            Llamar:5666401617
                        </a>
                    </div>
                </div>

            </div>

            <!-- Copyright -->
            <div class="pt-8 flex flex-col sm:flex-row justify-between items-center text-xs text-earth-muted gap-4">
                <p>&copy; 2026 Partido Macorina y El Peña. Todos los derechos reservados.</p>
                <p>Santa Isabel Ixtapan, Atenco, Edo. de Méx.</p>
            </div>
        </div>
    </footer>

    <!-- Inicializar Iconos -->
    <script>
        lucide.createIcons();
    </script>
</body>
</html
