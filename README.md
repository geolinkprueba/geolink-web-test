<!DOCTYPE html>
<html lang="es" class="dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Geolink V3.0 — Internet Inalámbrico de Alta Velocidad</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        darkBg: '#0b0f19',
                        cardBg: '#131c2e',
                        cyanAccent: '#00f2fe',
                        blueAccent: '#4facfe',
                    }
                }
            }
        }
    </script>
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Outfit', sans-serif; }
        .glow-cyan { box-shadow: 0 0 25px rgba(0, 242, 254, 0.25); }
        .glow-cyan-lg { box-shadow: 0 0 40px rgba(0, 242, 254, 0.4); }
    </style>
</head>
<body class="bg-[#0b0f19] text-slate-100 antialiased selection:bg-[#00f2fe] selection:text-black">

    <!-- HEADER / NAVEGACIÓN -->
    <header class="sticky top-0 z-50 backdrop-blur-xl bg-[#0b0f19]/80 border-b border-slate-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
            <div class="flex items-center space-x-3">
                <div class="w-10 h-10 rounded-xl bg-gradient-to-tr from-[#00f2fe] to-[#4facfe] flex items-center justify-center font-extrabold text-black text-xl glow-cyan">
                    G
                </div>
                <span class="text-2xl font-bold tracking-wider text-white">GEOLINK <span class="text-[#00f2fe] font-light text-lg">V3.0</span></span>
            </div>
            
            <nav class="hidden md:flex items-center space-x-8 text-sm font-medium text-slate-300">
                <a href="#planes" class="hover:text-[#00f2fe] transition">Planes Inalámbricos</a>
                <a href="#soporte" class="hover:text-[#00f2fe] transition">Soporte Local</a>
            </nav>

            <div class="flex items-center space-x-4">
                <a href="#planes" class="hidden sm:inline-flex items-center justify-center px-5 py-2.5 rounded-xl bg-gradient-to-r from-[#00f2fe] to-[#4facfe] text-black font-semibold text-sm hover:glow-cyan-lg transition">
                    Consultar Cobertura
                </a>
            </div>
        </div>
       <!-- SECCIÓN DE PREGUNTAS FRECUENTES (FAQ) & SOPORTE -->
    <section id="faq" class="py-24 bg-[#0b0f19] relative border-t border-slate-800/60">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-xs uppercase tracking-widest text-[#00f2fe] font-bold mb-3">Soporte y Transparencia</h2>
                <h3 class="text-3xl sm:text-4xl font-extrabold text-white">Preguntas Frecuentes sobre Geolink</h3>
                <p class="text-slate-400 mt-4">Todo lo que necesitas saber sobre nuestra tecnología inalámbrica fija (FWA), instalaciones en zonas urbanas y rurales de Girardota.</p>
            </div>

            <!-- ACORDEÓN DE PREGUNTAS -->
            <div class="space-y-4">
                
                <!-- Pregunta 1 -->
                <div class="bg-[#131c2e]/80 backdrop-blur rounded-2xl border border-slate-800 overflow-hidden transition">
                    <button onclick="toggleFaq(1)" class="w-full px-6 py-5 text-left flex justify-between items-center focus:outline-none">
                        <span class="font-bold text-white text-base">¿Cómo funciona el internet inalámbrico (FWA) en veredas y fincas?</span>
                        <span id="icon-1" class="text-[#00f2fe] font-extrabold text-xl transition-transform duration-300">+</span>
                    </button>
                    <div id="faq-1" class="hidden px-6 pb-5 text-sm text-slate-400 leading-relaxed border-t border-slate-800/50 pt-4">
                        Instalamos una antena receptora en un punto alto de tu propiedad con línea de vista directa (LOS) hacia nuestras estaciones base estratégicamente ubicadas en las montañas del norte del Aburrá. Esto garantiza una conexión robusta, de baja latencia y totalmente independiente del estado de las redes de cable tradicionales.
                    </div>
                </div>

                <!-- Pregunta 2 -->
                <div class="bg-[#131c2e]/80 backdrop-blur rounded-2xl border border-slate-800 overflow-hidden transition">
                    <button onclick="toggleFaq(2)" class="w-full px-6 py-5 text-left flex justify-between items-center focus:outline-none">
                        <span class="font-bold text-white text-base">¿Los planes residenciales (Línea Green) tienen cobro de IVA?</span>
                        <span id="icon-2" class="text-[#00f2fe] font-extrabold text-xl transition-transform duration-300">+</span>
                    </button>
                    <div id="faq-2" class="hidden px-6 pb-5 text-sm text-slate-400 leading-relaxed border-t border-slate-800/50 pt-4">
                        De acuerdo con la normatividad legal colombiana vigente, los servicios de internet domiciliario para estratos 1, 2 y 3 cuentan con beneficios tributarios (excluidos o con trato especial de IVA). Nuestros precios de la Línea Green reflejan el valor final para hogares.
                    </div>
                </div>

                <!-- Pregunta 3 -->
                <div class="bg-[#131c2e]/80 backdrop-blur rounded-2xl border border-slate-800 overflow-hidden transition">
                    <button onclick="toggleFaq(3)" class="w-full px-6 py-5 text-left flex justify-between items-center focus:outline-none">
                        <span class="font-bold text-white text-base">¿Cuál es el tiempo estimado de instalación en Girardota?</span>
                        <span id="icon-3" class="text-[#00f2fe] font-extrabold text-xl transition-transform duration-300">+</span>
                    </button>
                    <div id="faq-3" class="hidden px-6 pb-5 text-sm text-slate-400 leading-relaxed border-t border-slate-800/50 pt-4">
                        Una vez validada la viabilidad técnica de línea de vista en tu dirección o vereda, nuestras cuadrillas locales realizan la instalación profesional y configuración de la red Wi-Fi MESH en un plazo de 24 a 48 horas hábiles.
                    </div>
                </div>

                <!-- Pregunta 4 -->
                <div class="bg-[#131c2e]/80 backdrop-blur rounded-2xl border border-slate-800 overflow-hidden transition">
                    <button onclick="toggleFaq(4)" class="w-full px-6 py-5 text-left flex justify-between items-center focus:outline-none">
                        <span class="font-bold text-white text-base">¿Qué diferencia hay entre la Línea Green y la Línea Blue?</span>
                        <span id="icon-4" class="text-[#00f2fe] font-extrabold text-xl transition-transform duration-300">+</span>
                    </button>
                    <div id="faq-4" class="hidden px-6 pb-5 text-sm text-slate-400 leading-relaxed border-t border-slate-800/50 pt-4">
                        La <strong>Línea Green</strong> está diseñada para hogares, fincas y consumo residencial con tráfico ilimitado y tecnología WiFi Dual/MESH. La <strong>Línea Blue</strong> está orientada a comercios, empresas y centros de eventos en Girardota, e incluye condiciones fiscales con IVA y opciones de soporte prioritario empresarial o enlaces dedicados.
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- SCRIPT PARA EL ACORDEÓN DE FAQ -->
    <script>
        function toggleFaq(id) {
            const content = document.getElementById(`faq-${id}`);
            const icon = document.getElementById(`icon-${id}`);
            
            if (content.classList.contains('hidden')) {
                content.classList.remove('hidden');
                icon.innerText = "-";
            } else {
                content.classList.add('hidden');
                icon.innerText = "+";
            }
        }
    </script>

    </header>
        <!-- SECCIÓN DE COBERTURA INTERACTIVA -->
    <section id="cobertura" class="py-24 bg-[#0b0f19] relative border-t border-slate-800/60">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-xs uppercase tracking-widest text-[#00f2fe] font-bold mb-3">Infraestructura Regional</h2>
                <h3 class="text-3xl sm:text-4xl font-extrabold text-white">Cobertura Inalámbrica FWA en Girardota y el Norte del Aburrá</h3>
                <p class="text-slate-400 mt-4">Llevamos internet de alta velocidad con línea de vista directa (LOS) tanto al casco urbano como a veredas, sectores rurales y fincas de la región.</p>
            </div>

            <!-- GRID DE ZONAS Y VERIFICADOR -->
            <div class="grid lg:grid-cols-3 gap-8 items-stretch">
                
                <!-- ZONA URBANA -->
                <div class="bg-[#131c2e]/80 backdrop-blur rounded-3xl p-8 border border-slate-800 flex flex-col justify-between">
                    <div>
                        <div class="w-12 h-12 rounded-2xl bg-[#00f2fe]/10 flex items-center justify-center text-[#00f2fe] font-bold mb-6 text-xl">
                            🏙️
                        </div>
                        <h4 class="text-xl font-bold text-white mb-3">Casco Urbano Girardota</h4>
                        <p class="text-slate-400 text-sm mb-6">Conectividad robusta para hogares, conjuntos residenciales y locales comerciales en el área urbana con despliegue inmediato.</p>
                        <ul class="space-y-2 text-xs text-slate-300 mb-6">
                            <li class="flex items-center"><span class="text-[#00f2fe] mr-2">✓</span> Instalación prioritaria en 24-48h</li>
                            <li class="flex items-center"><span class="text-[#00f2fe] mr-2">✓</span> Estabilidad frente a cortes eléctricos</li>
                            <li class="flex items-center"><span class="text-[#00f2fe] mr-2">✓</span> Sin cruce de cables urbanos</li>
                        </ul>
                    </div>
                    <span class="inline-block px-3 py-1 bg-emerald-500/10 text-emerald-400 text-xs font-bold rounded-full w-fit">
                        Cobertura 100% Disponible
                    </span>
                </div>

                <!-- ZONA RURAL Y FINCAS -->
                <div class="bg-[#131c2e]/80 backdrop-blur rounded-3xl p-8 border border-slate-800 flex flex-col justify-between relative overflow-hidden">
                    <div class="absolute top-0 right-0 bg-[#00f2fe] text-black text-[10px] font-extrabold px-3 py-1 rounded-bl-xl uppercase">
                        Especialidad FWA
                    </div>
                    <div>
                        <div class="w-12 h-12 rounded-2xl bg-[#00f2fe]/10 flex items-center justify-center text-[#00f2fe] font-bold mb-6 text-xl">
                            🏡
                        </div>
                        <h4 class="text-xl font-bold text-white mb-3">Veredas, Fincas y Zonas Rurales</h4>
                        <p class="text-slate-400 text-sm mb-6">Llegamos donde la fibra tradicional no entra. Enlaces especializados de largo alcance con estaciones base de alta potencia en las montañas del norte del Aburrá.</p>
                        <ul class="space-y-2 text-xs text-slate-300 mb-6">
                            <li class="flex items-center"><span class="text-[#00f2fe] mr-2">✓</span> Enlaces punto a multipunto dedicados</li>
                            <li class="flex items-center"><span class="text-[#00f2fe] mr-2">✓</span> Ideal para descanso, trabajo remoto y cámaras</li>
                            <li class="flex items-center"><span class="text-[#00f2fe] mr-2">✓</span> Equipos industriales aptos para intemperie</li>
                        </ul>
                    </div>
                    <span class="inline-block px-3 py-1 bg-emerald-500/10 text-emerald-400 text-xs font-bold rounded-full w-fit">
                        Alta Demanda / Viabilidad por Vereda
                    </span>
                </div>

                <!-- TARJETA DE VERIFICACIÓN RÁPIDA -->
                <div class="bg-gradient-to-br from-[#131c2e] to-[#0b0f19] rounded-3xl p-8 border border-[#00f2fe]/30 flex flex-col justify-between shadow-lg shadow-[#00f2fe]/5">
                    <div>
                        <div class="w-12 h-12 rounded-2xl bg-[#00f2fe]/20 flex items-center justify-center text-[#00f2fe] font-bold mb-6 text-xl">
                            📡
                        </div>
                        <h4 class="text-xl font-bold text-white mb-2">Verifica tu Viabilidad</h4>
                        <p class="text-slate-400 text-sm mb-6">¿Estás en zona rural o finca? Nuestros técnicos validan la línea de vista satelital/inalámbrica con tus coordenadas o nombre de vereda.</p>
                        
                        <div class="space-y-3 mb-6">
                            <input type="text" id="verificacion-sector" placeholder="Escribe tu vereda, barrio o sector..." class="w-full bg-[#0b0f19] border border-slate-700 rounded-xl px-4 py-2.5 text-sm text-white placeholder-slate-500 focus:outline-none focus:border-[#00f2fe] transition">
                        </div>
                    </div>
                    
                    <button onclick="verificarViabilidad()" class="w-full py-3 rounded-xl bg-[#00f2fe] hover:bg-[#00d8e2] text-black font-extrabold text-sm transition shadow-lg shadow-[#00f2fe]/20 text-center">
                        Consultar Viabilidad por WhatsApp
                    </button>
                </div>

            </div>
        </div>
    </section>

    <!-- SCRIPT DE INTERACCIÓN RÁPIDA PARA WHATSAPP -->
    <script>
        function verificarViabilidad() {
            const sector = document.getElementById('verificacion-sector').value.trim();
            const mensaje = sector 
                ? `Hola Geolink, quiero verificar la viabilidad técnica de internet para el sector/vereda: ${sector}`
                : `Hola Geolink, quiero verificar la disponibilidad de cobertura en Girardota.`;
            const urlWhatsApp = `https://wa.me/573000000000?text=${encodeURIComponent(mensaje)}`;
            window.open(urlWhatsApp, '_blank');
        }
    </script>


    <!-- HERO SECTION -->
    <section class="relative pt-20 pb-32 overflow-hidden">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid lg:grid-cols-12 gap-12 items-center">
                <div class="lg:col-span-7 space-y-6 text-center lg:text-left">
                    <div class="inline-flex items-center space-x-2 px-3.5 py-1.5 rounded-full bg-slate-900 border border-slate-700 text-xs text-[#00f2fe] font-medium">
                        <span class="w-2 h-2 rounded-full bg-[#00f2fe] animate-pulse"></span>
                        <span>100% Tecnología Inalámbrica de Alta Capacidad (Sin Falsas Fibras)</span>
                    </div>
                    <h1 class="text-4xl sm:text-6xl font-extrabold tracking-tight text-white leading-tight">
                        INTERNET INALÁMBRICO QUE <span class="text-transparent bg-clip-text bg-gradient-to-r from-[#00f2fe] to-[#4facfe]">FUNCIONA DONDE OTROS NO LLEGAN.</span>
                    </h1>
                    <p class="text-lg text-slate-300 max-w-2xl mx-auto lg:mx-0">
                        Conectividad robusta y estable para hogares, fincas y comercios en Girardota y el norte del Valle de Aburrá. Cero cables, cero barreras geográficas y sin contratos largos.
                    </p>
                    <div class="flex flex-col sm:flex-row items-center justify-center lg:justify-start space-y-4 sm:space-y-0 sm:space-x-4 pt-4">
                        <a href="#planes" class="w-full sm:w-auto px-8 py-4 rounded-xl bg-[#00f2fe] text-black font-bold text-center hover:glow-cyan-lg transition">
                            Ver Planes Inalámbricos
                        </a>
                    </div>
                </div>
                <div class="lg:col-span-5">
                    <div class="relative rounded-3xl p-1 bg-gradient-to-tr from-[#00f2fe] to-[#4facfe] glow-cyan">
                        <div class="bg-[#131c2e] rounded-[22px] p-6 space-y-6">
                            <div class="flex items-center justify-between border-b border-slate-800 pb-4">
                                <span class="text-sm font-semibold text-slate-400">ESTADO DE RED REGIONAL</span>
                                <span class="px-2.5 py-1 rounded-md bg-emerald-500/10 text-emerald-400 text-xs font-semibold">100% Operativo</span>
                            </div>
                            <div class="space-y-4">
                                <div class="flex items-center justify-between text-sm">
                                    <span class="text-slate-300">Estación Base Girardota</span>
                                    <span class="text-[#00f2fe] font-mono">Latencia 6ms</span>
                                </div>
                                <div class="w-full bg-slate-800 h-2 rounded-full overflow-hidden">
                                    <div class="bg-gradient-to-r from-[#00f2fe] to-[#4facfe] h-full w-[95%]"></div>
                                </div>
                            </div>
                            <div class="p-4 rounded-xl bg-slate-900/60 border border-slate-800 text-xs text-slate-400">
                                📡 Cobertura garantizada por línea de vista directa con equipos de última generación.
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- SELECTOR INTELIGENTE DE PLANES INALÁMBRICOS -->
            <!-- SMART PLAN SELECTOR -->
    <section id="planes" class="py-24 bg-[#0b0f19] relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-xs uppercase tracking-widest text-[#00f2fe] font-bold mb-3">Selector Inteligente de Planes</h2>
                <h3 class="text-3xl sm:text-4xl font-extrabold text-white">Conectividad de Alta Capacidad en Girardota</h3>
                <p class="text-slate-400 mt-4">Información basada en la oferta oficial de Geolink: Línea Green residencial y Línea Blue comercial con especificaciones reales.</p>
            </div>

            <!-- GRID DE PLANES -->
            <div class="grid lg:grid-cols-2 gap-8 items-start">
                
                <!-- COLUMNA RESIDENCIAL (LÍNEA GREEN) -->
                <div class="bg-[#131c2e]/80 backdrop-blur rounded-3xl p-8 border border-slate-800 relative">
                    <div class="absolute -top-3 left-8 bg-[#00f2fe] text-black text-xs font-extrabold px-3 py-1 rounded-full uppercase">
                        Línea Green (Residencial) • Tráfico Ilimitado
                    </div>
                    <h4 class="text-2xl font-bold text-white mt-4 mb-2">Hogar & Fincas</h4>
                    <p class="text-slate-400 text-sm mb-6">Conectividad estable con Wi-Fi Dual Band y tecnología MESH para zonas urbanas y rurales.</p>

                    <div class="space-y-4">
                        <!-- Green 15M -->
                        <div class="p-4 rounded-2xl bg-[#0b0f19] border border-slate-800/80 flex items-center justify-between">
                            <div>
                                <span class="text-xs text-[#00f2fe] font-semibold">GREEN 15M</span>
                                <h5 class="text-xl font-bold text-white">15 Mbps</h5>
                                <p class="text-xs text-slate-400">Soporte hasta 10 dispositivos • 1 Zona WiFi Dual</p>
                            </div>
                            <div class="text-right">
                                <span class="text-lg font-extrabold text-white">$97.500 <span class="text-xs text-slate-400">/mes</span></span>
                                <a href="https://wa.me/573000000000?text=Hola%20Geolink,%20quiero%20el%20Plan%20Green%2015M" target="_blank" class="block mt-2 px-4 py-1.5 rounded-lg bg-[#00f2fe]/10 hover:bg-[#00f2fe] text-[#00f2fe] hover:text-black font-bold text-xs transition">Seleccionar</a>
                            </div>
                        </div>

                        <!-- Green 30M -->
                        <div class="p-4 rounded-2xl bg-[#0b0f19] border border-slate-800/80 flex items-center justify-between">
                            <div>
                                <span class="text-xs text-[#00f2fe] font-semibold">GREEN 30M</span>
                                <h5 class="text-xl font-bold text-white">30 Mbps</h5>
                                <p class="text-xs text-slate-400">Soporte hasta 15 dispositivos • 2 Zonas WiFi MESH</p>
                            </div>
                            <div class="text-right">
                                <span class="text-lg font-extrabold text-white">$127.500 <span class="text-xs text-slate-400">/mes</span></span>
                                <a href="https://wa.me/573000000000?text=Hola%20Geolink,%20quiero%20el%20Plan%20Green%2030M" target="_blank" class="block mt-2 px-4 py-1.5 rounded-lg bg-[#00f2fe]/10 hover:bg-[#00f2fe] text-[#00f2fe] hover:text-black font-bold text-xs transition">Seleccionar</a>
                            </div>
                        </div>

                        <!-- Green 50M -->
                        <div class="p-4 rounded-2xl bg-[#0b0f19] border border-slate-800/80 flex items-center justify-between">
                            <div>
                                <span class="text-xs text-[#00f2fe] font-semibold">GREEN 50M</span>
                                <h5 class="text-xl font-bold text-white">50 Mbps</h5>
                                <p class="text-xs text-slate-400">Soporte hasta 25 dispositivos • WiFi Dual Band</p>
                            </div>
                            <div class="text-right">
                                <span class="text-lg font-extrabold text-white">$154.500 <span class="text-xs text-slate-400">/mes</span></span>
                                <a href="https://wa.me/573000000000?text=Hola%20Geolink,%20quiero%20el%20Plan%20Green%2050M" target="_blank" class="block mt-2 px-4 py-1.5 rounded-lg bg-[#00f2fe]/10 hover:bg-[#00f2fe] text-[#00f2fe] hover:text-black font-bold text-xs transition">Seleccionar</a>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- COLUMNA COMERCIAL / CORPORATIVO (LÍNEA BLUE) -->
                <div class="bg-[#131c2e]/80 backdrop-blur rounded-3xl p-8 border border-slate-800 relative">
                    <div class="absolute -top-3 left-8 bg-amber-400 text-black text-xs font-extrabold px-3 py-1 rounded-full uppercase">
                        Línea Blue (Comercial & Corporativo)
                    </div>
                    <h4 class="text-2xl font-bold text-white mt-4 mb-2">Negocios y Empresas</h4>
                    <p class="text-slate-400 text-sm mb-6">Soluciones avanzadas, innovación en centros de eventos y soporte especializado para empresas.</p>

                    <div class="space-y-4">
                        <!-- Blue 50M -->
                        <div class="p-4 rounded-2xl bg-[#0b0f19] border border-slate-800/80 flex items-center justify-between">
                            <div>
                                <span class="text-xs text-amber-400 font-semibold">BLUE 50M</span>
                                <h5 class="text-xl font-bold text-white">50 Mbps</h5>
                                <p class="text-xs text-slate-400">Centros de eventos • Gestión de visitantes</p>
                            </div>
                            <div class="text-right">
                                <span class="text-lg font-extrabold text-white">$194.600 <span class="text-xs text-slate-400">+ IVA</span></span>
                                <a href="https://wa.me/573000000000?text=Hola%20Geolink,%20quiero%20el%20Plan%20Blue%2050M" target="_blank" class="block mt-2 px-4 py-1.5 rounded-lg bg-amber-400/10 hover:bg-amber-400 text-amber-400 hover:text-black font-bold text-xs transition">Seleccionar</a>
                            </div>
                        </div>

                        <!-- Blue 100M -->
                        <div class="p-4 rounded-2xl bg-[#0b0f19] border border-slate-800/80 flex items-center justify-between">
                            <div>
                                <span class="text-xs text-amber-400 font-semibold">BLUE 100M</span>
                                <h5 class="text-xl font-bold text-white">100 Mbps</h5>
                                <p class="text-xs text-slate-400">Solución integral • Soporte técnico 24/7</p>
                            </div>
                            <div class="text-right">
                                <span class="text-lg font-extrabold text-white">$250.000 <span class="text-xs text-slate-400">+ IVA</span></span>
                                <a href="https://wa.me/573000000000?text=Hola%20Geolink,%20quiero%20el%20Plan%20Blue%20100M" target="_blank" class="block mt-2 px-4 py-1.5 rounded-lg bg-amber-400/10 hover:bg-amber-400 text-amber-400 hover:text-black font-bold text-xs transition">Seleccionar</a>
                            </div>
                        </div>

                        <!-- Enlace Dedicado -->
                        <div class="p-4 rounded-2xl bg-[#0b0f19] border border-slate-800/80 flex items-center justify-between">
                            <div>
                                <span class="text-xs text-amber-400 font-semibold">ENLACE DEDICADO</span>
                                <h5 class="text-xl font-bold text-white">Punto a Punto</h5>
                                <p class="text-xs text-slate-400">Hasta 100M simétricos y baja latencia</p>
                            </div>
                            <div class="text-right">
                                <span class="text-lg font-extrabold text-white">A Medida</span>
                                <a href="https://wa.me/573000000000?text=Hola%20Geolink,%20quiero%20consultar%20sobre%20Enlace%20Punto%20a%20Punto" target="_blank" class="block mt-2 px-4 py-1.5 rounded-lg bg-amber-400/10 hover:bg-amber-400 text-amber-400 hover:text-black font-bold text-xs transition">Consultar</a>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>


    <!-- SOPORTE LOCAL Y WHATSAPP DIRECTO -->
    <section id="soporte" class="py-24 bg-[#0b0f19] border-t border-slate-800/80">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid lg:grid-cols-12 gap-12 items-center">
                <div class="lg:col-span-6 space-y-6">
                    <div class="inline-flex items-center space-x-2 px-3 py-1 rounded-full bg-emerald-500/10 border border-emerald-500/20 text-xs text-emerald-400 font-medium">
                        <span class="w-2 h-2 rounded-full bg-emerald-400 animate-pulse"></span>
                        <span>Atención Humana y Local en Girardota</span>
                    </div>
                    <h2 class="text-3xl sm:text-4xl font-extrabold text-white">¿Dudas sobre cobertura o tu sector específico?</h2>
                    <p class="text-slate-300">
                        No tratamos con centrales automáticas lejanas. Habla directamente con nuestro equipo técnico local para validar la línea de vista de tu hogar, finca o negocio de forma inmediata.
                    </p>
                    <div class="space-y-4 pt-2">
                        <div class="flex items-center space-x-3 text-slate-300 text-sm">
                            <div class="w-8 h-8 rounded-lg bg-[#00f2fe]/10 flex items-center justify-center text-[#00f2fe] font-bold">✓</div>
                            <span>Visita técnica y diagnóstico de línea de vista</span>
                        </div>
                        <div class="flex items-center space-x-3 text-slate-300 text-sm">
                            <div class="w-8 h-8 rounded-lg bg-[#00f2fe]/10 flex items-center justify-center text-[#00f2fe] font-bold">✓</div>
                            <span>Instalación rápida adaptada a tu zona (Urbana o Veredal)</span>
                        </div>
                    </div>
                </div>

                <div class="lg:col-span-6">
                    <div class="bg-[#131c2e] rounded-3xl p-8 border border-slate-800 glow-cyan relative overflow-hidden">
                        <div class="absolute -right-10 -bottom-10 w-40 h-40 bg-[#00f2fe]/10 rounded-full blur-3xl"></div>
                        <h3 class="text-2xl font-bold text-white mb-4">Canal Directo de Ventas</h3>
                        <p class="text-slate-400 text-sm mb-8">
                            Haz clic en el botón para iniciar una conversación inmediata por WhatsApp con un asesor técnico de Geolink.
                        </p>
                        <a href="https://wa.me/573000000000?text=Hola%20Geolink,%20quiero%20consultar%20cobertura%20e%20internet%20inalámbrico%20en%20Girardota" target="_blank" class="flex items-center justify-center space-x-3 w-full py-4 rounded-xl bg-emerald-500 hover:bg-emerald-400 text-black font-extrabold text-center transition shadow-lg shadow-emerald-500/20">
                            <span class="text-xl">💬</span>
                            <span>Abrir Chat de WhatsApp Directo</span>
                        </a>
                        <p class="text-xs text-slate-500 text-center mt-4">Respuesta rápida en horario hábil regional.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="bg-[#070a12] border-t border-slate-800/80 py-8 text-center text-xs text-slate-500">
        <p>© 2026 Geolink S.A.S. Entorno de Pruebas Privado.</p>
    </footer>

</body>
</html>
