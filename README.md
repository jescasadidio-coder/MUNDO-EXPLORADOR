<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mundo Explorador - Modo CyT</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Fredoka:wght@400;600&display=swap');
        body { font-family: 'Fredoka', sans-serif; }

        .logo-box { height: 60px; width: 140px; background-size: contain; background-position: center; background-repeat: no-repeat; }
        .logo-modo-cyt { background-image: url('./logo-modo-cyt.png'); }
        .logo-agencia { background-image: url('./logo-agencia.png'); }

        .card-img-container { height: 160px; background-size: cover; background-position: center; background-repeat: no-repeat; background-color: #e5e7eb; }
        
        /* RUTAS RELATIVAS (Asegurate que el nombre coincida EXACTO en GitHub) */
        .img-inicial { background-image: url('./inicial.jpg'); }
        .img-matriz-led { background-image: url('./matriz-led.png'); }
        .img-circuitos-luz { background-image: url('./circuitos-luz.png'); }
        .img-huerta-inteligente { background-image: url('./huerta-inteligente.png'); }
        .img-auto-control-remoto { background-image: url('./auto-control-remoto.png'); }
        .img-otros { background-image: url('./otros.jpg'); }

        .accordion-content { max-height: 0; overflow: hidden; transition: max-height 0.5s ease-out; }
        .active .accordion-content { max-height: 1000px; }
        .label-nivel { font-size: 0.7rem; font-weight: bold; padding: 2px 8px; border-radius: 4px; display: inline-block; margin-bottom: 8px; }
    </style>
</head>
<body class="bg-[#f0f4f8] p-4 md:p-8 text-[#1d3557]">

    <div class="max-w-7xl mx-auto">
        <header class="bg-white rounded-2xl shadow-sm p-6 mb-8 flex flex-col md:flex-row justify-between items-center gap-4 border-b-4 border-[#1d3557]">
            <div>
                <h1 class="text-3xl font-bold uppercase tracking-tight">Mundo Explorador</h1>
                <p class="text-[#457b9d] font-semibold italic">Programa ConciencIA en tu Escuela</p>
            </div>
            <div class="flex items-center gap-6">
                <div class="logo-box logo-modo-cyt"></div>
                <div class="logo-box logo-agencia"></div>
            </div>
        </header>

        <section class="bg-[#1d3557] text-white rounded-3xl p-6 mb-10 shadow-lg">
            <h3 class="text-xl font-bold mb-2 text-[#a8dadc]">🚀 Sobre el Programa</h3>
            <p class="text-sm opacity-90 leading-relaxed">
                Propuestas de la Secretaría de Ciencia y Tecnología para democratizar el acceso al conocimiento digital y hardware abierto en Tierra del Fuego.
            </p>
        </section>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            <div class="bg-white rounded-3xl overflow-hidden shadow-md border-t-8 border-[#a8dadc] card-container">
                <div class="card-img-container img-inicial"></div>
                <div class="p-6">
                    <span class="label-nivel bg-[#a8dadc]">NIVEL INICIAL</span>
                    <h2 class="text-lg font-bold mb-4 uppercase">Buscadores de Colores</h2>
                    <button onclick="toggleCard(this)" class="w-full bg-[#f1faee] py-2 rounded-xl font-semibold hover:bg-[#a8dadc]">DETALLES ▼</button>
                    <div class="accordion-content text-sm text-gray-600 mt-4 space-y-2">
                        <p><strong>🎯 Finalidad:</strong> Inquietud científica mediante fotosensibilidad.</p>
                        <p><strong>🛠️ Descripción:</strong> Antotipia y mediación de IA.</p>
                    </div>
                </div>
            </div>

            <div class="bg-white rounded-3xl overflow-hidden shadow-md border-t-8 border-[#457b9d] card-container">
                <div class="card-img-container img-matriz-led"></div>
                <div class="p-6">
                    <span class="label-nivel bg-[#457b9d] text-white">PRIMARIA - OPCIÓN A</span>
                    <h2 class="text-lg font-bold mb-4 uppercase">Dibujos en Matriz LED</h2>
                    <button onclick="toggleCard(this)" class="w-full bg-[#f1faee] py-2 rounded-xl font-semibold hover:bg-[#a8dadc]">DETALLES ▼</button>
                    <div class="accordion-content text-sm text-gray-600 mt-4 space-y-2">
                        <p><strong>🎯 Finalidad:</strong> Alfabetización digital y hardware abierto.</p>
                        <p><strong>🛠️ Descripción:</strong> Uso de placas Archi para diseño LED.</p>
                    </div>
                </div>
            </div>

            <div class="bg-white rounded-3xl overflow-hidden shadow-md border-t-8 border-[#457b9d] card-container">
                <div class="card-img-container img-circuitos-luz"></div>
                <div class="p-6">
                    <span class="label-nivel bg-[#457b9d] text-white">PRIMARIA - OPCIÓN B</span>
                    <h2 class="text-lg font-bold mb-4 uppercase">Circuitos de Luz</h2>
                    <button onclick="toggleCard(this)" class="w-full bg-[#f1faee] py-2 rounded-xl font-semibold hover:bg-[#a8dadc]">DETALLES ▼</button>
                    <div class="accordion-content text-sm text-gray-600 mt-4 space-y-2">
                        <p><strong>🎯 Finalidad:</strong> Electrónica básica y experimentación artística.</p>
                        <p><strong>🛠️ Descripción:</strong> Construcción de circuitos creativos.</p>
                    </div>
                </div>
            </div>

            <div class="bg-white rounded-3xl overflow-hidden shadow-md border-t-8 border-[#1d3557] card-container">
                <div class="card-img-container img-huerta-inteligente"></div>
                <div class="p-6">
                    <span class="label-nivel bg-[#1d3557] text-white">SECUNDARIA - OPCIÓN A</span>
                    <h2 class="text-lg font-bold mb-4 uppercase">Huerta Inteligente</h2>
                    <button onclick="toggleCard(this)" class="w-full bg-[#f1faee] py-2 rounded-xl font-semibold hover:bg-[#a8dadc]">DETALLES ▼</button>
                    <div class="accordion-content text-sm text-gray-600 mt-4 space-y-2">
                        <p><strong>🎯 Finalidad:</strong> Automatización de recursos naturales.</p>
                        <p><strong>🛠️ Descripción:</strong> Monitoreo de humedad y temperatura con sensores.</p>
                    </div>
                </div>
            </div>

            <div class="bg-white rounded-3xl overflow-hidden shadow-md border-t-8 border-[#1d3557] card-container">
                <div class="card-img-container img-auto-control-remoto"></div>
                <div class="p-6">
                    <span class="label-nivel bg-[#1d3557] text-white">SECUNDARIA - OPCIÓN B</span>
                    <h2 class="text-lg font-bold mb-4 uppercase">Auto Control Remoto</h2>
                    <button onclick="toggleCard(this)" class="w-full bg-[#f1faee] py-2 rounded-xl font-semibold hover:bg-[#a8dadc]">DETALLES ▼</button>
                    <div class="accordion-content text-sm text-gray-600 mt-4 space-y-2">
                        <p><strong>🎯 Finalidad:</strong> Robótica móvil y control físico.</p>
                        <p><strong>🛠️ Descripción:</strong> Ensamblaje y programación de vehículos.</p>
                    </div>
                </div>
            </div>

            <div class="bg-white rounded-3xl overflow-hidden shadow-md border-t-8 border-gray-400 card-container">
                <div class="card-img-container img-otros"></div>
                <div class="p-6">
                    <span class="label-nivel bg-gray-400 text-white">COMUNIDAD</span>
                    <h2 class="text-lg font-bold mb-4 uppercase">Mentorías</h2>
                    <button onclick="toggleCard(this)" class="w-full bg-[#f1faee] py-2 rounded-xl font-semibold hover:bg-[#a8dadc]">DETALLES ▼</button>
                    <div class="accordion-content text-sm text-gray-600 mt-4 space-y-2">
                        <p><strong>🤝 Vínculo:</strong> Mentorías y formación docente a medida.</p>
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
