# geolink-web-test
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
                <a href="#tecnologia" class="hover:text-[#00f2fe] transition">Tecnología FWA / WiMAX</a>
                <a href="#soporte" class="hover:text-[#00f2fe] transition">Soporte Local</a>
            </nav>

            <div class="flex items-center space-x-4">
                <a href="#planes" class="hidden sm:inline-flex items-center justify-center px-5 py-2.5 rounded-xl bg-gradient-to-r from-[#00f2fe] to-[#4facfe] text-black font-semibold text-sm hover:glow-cyan-lg transition">
                    Consultar Cobertura
                </a>
            </div>
        </div>
    </header>

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
                                📡 Cobertura garantizada por línea de vista directa con equipos CPE de última generación.
                            </div>
                        </div>
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
