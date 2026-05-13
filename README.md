<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mundo Explorador</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Fredoka:wght@400;600&display=swap');
        body { font-family: 'Fredoka', sans-serif; }

        .logo-box { height: 60px; width: 140px; background-size: contain; background-position: center; background-repeat: no-repeat; }
        /* RUTAS DIRECTAS (SIN CARPETAS) */
        .logo-modo-cyt { background-image: url('logo-modo-cyt.png'); }
        .logo-agencia { background-image: url('logo-agencia.png'); }

        .card-img-container { height: 180px; background-size: cover; background-position: center; background-repeat: no-repeat; background-color: #f3f4f6; }
        
        .img-inicial { background-image: url('inicial.jpg'); }
        .img-matriz-led { background-image: url('matriz-led.png'); }
        .img-circuitos-luz { background-image: url('circuitos-luz.png'); }
        .img-huerta-inteligente { background-image: url('huerta-inteligente.png'); }
        .img-auto-control-remoto { background-image: url('auto-control-remoto.png'); }
        .img-otros { background-image: url('otros.jpg'); }

        .accordion-content { max-height: 0; overflow: hidden; transition: max-height 0.5s ease-out; }
        .active .accordion-content { max-height: 1000px; padding-top: 1rem; }
        .label-nivel { font-size: 0.7rem; font-weight: bold; padding: 2px 8px; border-radius: 4px; display: inline-block; margin-bottom: 8px; }
    </style>
</head>
<body class="bg-[#f0f4f8] p-4 md:p-8 text-[#1d3557]">

    <div class="max-w-7xl mx-auto">
        <header class="bg-white rounded-2xl shadow-sm p-6 mb-8 flex flex-col md:flex-row justify-between items-center gap-4 border-b-4 border-[#1d3557]">
            <div class="text-center md:text-left">
                <h1 class="text-3xl font-bold uppercase tracking-tight">Mundo Explorador</h1>
                <p class="text-[#457b9d] font-semibold italic">Programa ConciencIA en tu Escuela</p>
            </div>
            <div class="flex items-center gap-6">
                <div class="logo-box logo-modo-cyt"></div>
                <div class="logo-box logo-agencia"></div>
            </div>
        </header>

        <section class="bg-[#1d3557] text-white rounded-3xl p-6 mb-10 shadow-lg">
            <h3 class="text-xl font-bold mb-2 text-[#a8dadc]">🚀 ¡Bienvenidos, Exploradores!</h3>
            <p class="text-sm opacity-90">Secretaría de Ciencia y Tecnología - Tierra del Fuego.</p>
        </section>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            <div class="bg-white rounded-3xl overflow-hidden shadow-md border-t-8 border-[#a8dadc] card-container">
                <div class="card-img-container img-inicial"></div>
                <div class="p-6">
                    <span class="label-nivel bg-[#a8dadc]">NIVEL INICIAL</span>
                    <h2 class="text-lg font-bold mb-4 uppercase">Buscadores de Colores</h2>
                    <button onclick="toggleCard(this)" class="w-full bg-[#f1faee] py-2 rounded-xl font-semibold">VER MÁS ▼</button>
                    <div class="accordion-content text-sm text-gray-600">
                        <p>Exploración del entorno mediante procesos creativos y fotosensibilidad.</p>
                    </div>
                </div>
            </div>

            <div class="bg-white rounded-3xl overflow-hidden shadow-md border-t-8 border-[#457b9d] card-container">
                <div class="card-img-container img-matriz-led"></div>
                <div class="p-6">
                    <span class="label-nivel bg-[#457b9d] text-white">PRIMARIA - A</span>
                    <h2 class="text-lg font-bold mb-4 uppercase">Dibujos en Matriz LED</h2>
                    <button onclick="toggleCard(this)" class="w-full bg-[#f1faee] py-2 rounded-xl font-semibold">VER MÁS ▼</button>
                    <div class="accordion-content text-sm text-gray-600">
                        <p>Programación visual y hardware abierto con placas Archi.</p>
                    </div>
                </div>
            </div>

            <div class="bg-white rounded-3xl overflow-hidden shadow-md border-t-8 border-[#457b9d] card-container">
                <div class="card-img-container img-circuitos-luz"></div>
                <div class="p-6">
                    <span class="label-nivel bg-[#457b9d] text-white">PRIMARIA - B</span>
                    <h2 class="text-lg font-bold mb-4 uppercase">Circuitos de Luz</h2>
                    <button onclick="toggleCard(this)" class="w-full bg-[#f1faee] py-2 rounded-xl font-semibold">VER MÁS ▼</button>
                    <div class="accordion-content text-sm text-gray-600">
                        <p>Electrónica básica para instalaciones artísticas con luz y sombra.</p>
                    </div>
                </div>
            </div>

            <div class="bg-white rounded-3xl overflow-hidden shadow-md border-t-8 border-[#1d3557] card-container">
                <div class="card-img-container img-huerta-inteligente"></div>
                <div class="p-6">
                    <span class="label-nivel bg-[#1d3557] text-white">SECUNDARIA - A</span>
                    <h2 class="text-lg font-bold mb-4 uppercase">Huerta Inteligente</h2>
                    <button onclick="toggleCard(this)" class="w-full bg-[#f1faee] py-2 rounded-xl font-semibold">VER MÁS ▼</button>
                    <div class="accordion-content text-sm text-gray-600">
                        <p>Automatización y monitoreo de recursos con sensores de humedad.</p>
                    </div>
                </div>
            </div>

            <div class="bg-white rounded-3xl overflow-hidden shadow-md border-t-8 border-[#1d3557] card-container">
                <div class="card-img-container img-auto-control-remoto"></div>
                <div class="p-6">
                    <span class="label-nivel bg-[#1d3557] text-white">SECUNDARIA - B</span>
                    <h2 class="text-lg font-bold mb-4 uppercase">Robótica Móvil</h2>
                    <button onclick="toggleCard(this)" class="w-full bg-[#f1faee] py-2 rounded-xl font-semibold">VER MÁS ▼</button>
                    <div class="accordion-content text-sm text-gray-600">
                        <p>Ensamblaje y programación de vehículos electrónicos remotos.</p>
                    </div>
                </div>
            </div>

            <div class="bg-white rounded-3xl overflow-hidden shadow-md border-t-8 border-gray-400 card-container">
                <div class="card-img-container img-otros"></div>
                <div class="p-6">
                    <span class="label-nivel bg-gray-400 text-white">FORMACIÓN</span>
                    <h2 class="text-lg font-bold mb-4 uppercase">Mentorías</h2>
                    <button onclick="toggleCard(this)" class="w-full bg-[#f1faee] py-2 rounded-xl font-semibold">VER MÁS ▼</button>
                    <div class="accordion-content text-sm text-gray-600">
                        <p>Acompañamiento a docentes en proyectos tecnológicos.</p>
                    </div>
                </div>
            </div>
        </div>

        <div class="mt-16 text-center">
            <a href="https://forms.gle/rwDH4E9ny6HjjNEY8" target="_blank" class="bg-[#e63946] text-white text-2xl font-bold py-5 px-14 rounded-full shadow-2xl inline-block hover:scale-105 transition-all">
                ¡INSCRIBIR MI ESCUELA! 🚀
            </a>
        </div>
    </div>

    <script>
        function toggleCard(button) {
            const container = button.closest('.card-container');
            container.classList.toggle('active');
        }
    </script>
</body>
</html>
