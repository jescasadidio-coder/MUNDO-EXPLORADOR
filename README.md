# MUNDO-EXPLORADOR
Iniciativa de la Secretaría de Ciencia y Tecnología para integrar contenidos de educación digital, hardware y procesos naturales. Buscamos democratizar el acceso tecnológico en Tierra del Fuego con una mirada crítica y soberana.
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

        /* --- CONFIGURACIÓN DE IMÁGENES --- */
        .logo-box { height: 60px; width: 140px; background-size: contain; background-position: center; background-repeat: no-repeat; }
        .logo-modo-cyt { background-image: url('logo-modo-cyt.png'); }
        .logo-agencia { background-image: url('logo-agencia.png'); }

        .card-img-container { height: 180px; background-size: cover; background-position: center; background-repeat: no-repeat; background-color: #e5e7eb; }
        .img-foto-inicial { background-image: url('inicial.jpg'); }
        .img-foto-primaria { background-image: url('primaria.jpg'); }
        .img-foto-secundaria { background-image: url('secundaria.jpg'); }
        .img-foto-otros { background-image: url('otros.jpg'); }

        .accordion-content { max-height: 0; overflow: hidden; transition: max-height 0.5s ease-out; }
        .active .accordion-content { max-height: 1200px; }
    </style>
</head>
<body class="bg-[#f0f4f8] p-4 md:p-8">

    <div class="max-w-6xl mx-auto">
        <header class="bg-white rounded-2xl shadow-sm p-6 mb-6 flex flex-col md:flex-row justify-between items-center gap-4 border-b-4 border-[#1d3557]">
            <div class="text-center md:text-left">
                <h1 class="text-3xl font-bold text-[#1d3557]">MUNDO EXPLORADOR</h1>
                <p class="text-[#457b9d] font-semibold">Programa ConciencIA en tu Escuela</p>
            </div>
            <div class="flex items-center gap-6">
                <div class="logo-box logo-modo-cyt"></div>
                <div class="h-10 w-px bg-gray-200 hidden md:block"></div>
                <div class="logo-box logo-agencia"></div>
            </div>
        </header>

        <section class="bg-[#1d3557] text-white rounded-3xl p-6 mb-8 shadow-lg">
            <h3 class="text-xl font-bold mb-2 text-[#a8dadc]">🚀 Sobre el Programa</h3>
            <p class="text-sm leading-relaxed opacity-90">
                Iniciativa de la Secretaría de Ciencia y Tecnología para integrar contenidos de educación digital, hardware y procesos naturales. Buscamos democratizar el acceso tecnológico en Tierra del Fuego con una mirada crítica y soberana.
            </p>
        </section>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
            
            <div class="bg-white rounded-3xl overflow-hidden shadow-md border-t-8 border-[#a8dadc] card-container">
                <div class="card-img-container img-foto-inicial"></div>
                <div class="p-5">
                    <h2 class="text-xl font-bold text-center mb-4 text-[#1d3557]">INICIAL</h2>
                    <button onclick="toggleCard(this)" class="w-full bg-[#f1faee] py-2 rounded-xl font-semibold text-[#1d3557] hover:bg-[#a8dadc] transition-colors">VER DETALLES ▼</button>
                    <div class="accordion-content">
                        <div class="py-4 px-2 text-gray-600 text-xs space-y-3">
                            <p><strong>🎯 Finalidad:</strong> Incentivar la inquietud científica mediante la fotosensibilidad y el entorno natural.</p>
                            <p><strong>🛠️ Taller:</strong> Antotipia (Buscadores de Colores) y Sombras Mágicas.</p>
                            <p><strong>📅 Días:</strong> Lunes y Miércoles (Mañana/Tarde).</p>
                        </div>
                    </div>
                </div>
            </div>

            <div class="bg-white rounded-3xl overflow-hidden shadow-md border-t-8 border-[#457b9d] card-container">
                <div class="card-img-container img-foto-primaria"></div>
                <div class="p-5">
                    <h2 class="text-xl font-bold text-center mb-4 text-[#1d3557]">PRIMARIA</h2>
                    <button onclick="toggleCard(this)" class="w-full bg-[#f1faee] py-2 rounded-xl font-semibold text-[#1d3557] hover:bg-[#a8dadc] transition-colors">VER DETALLES ▼</button>
                    <div class="accordion-content">
                        <div class="py-4 px-2 text-gray-600 text-xs space-y-3">
                            <p><strong>🎯 Finalidad:</strong> Alfabetización digital y control de hardware abierto.</p>
                            <p><strong>🛠️ Talleres:</strong> Matriz LED con placas Archi y Circuitos de Luz.</p>
                            <p><strong>📅 Días:</strong> Martes y Jueves.</p>
                        </div>
                    </div>
                </div>
            </div>

            <div class="bg-white rounded-3xl overflow-hidden shadow-md border-t-8 border-[#1d3557] card-container">
                <div class="card-img-container img-foto-secundaria"></div>
                <div class="p-5">
                    <h2 class="text-xl font-bold text-center mb-4 text-[#1d3557]">SECUNDARIA</h2>
                    <button onclick="toggleCard(this)" class="w-full bg-[#f1faee] py-2 rounded-xl font-semibold text-[#1d3557] hover:bg-[#a8dadc] transition-colors">VER DETALLES ▼</button>
                    <div class="accordion-content">
                        <div class="py-4 px-2 text-gray-600 text-xs space-y-3">
                            <p><strong>🎯 Finalidad:</strong> Robótica móvil y automatización de recursos naturales.</p>
                            <p><strong>🛠️ Talleres:</strong> Huerta Inteligente y Auto a Control Remoto.</p>
                            <p><strong>📅 Días:</strong> Viernes.</p>
                        </div>
                    </div>
                </div>
            </div>

            <div class="bg-white rounded-3xl overflow-hidden shadow-md border-t-8 border-gray-400 card-container">
                <div class="card-img-container img-foto-otros"></div>
                <div class="p-5">
                    <h2 class="text-xl font-bold text-center mb-4 text-[#1d3557]">OTROS</h2>
                    <button onclick="toggleCard(this)" class="w-full bg-[#f1faee] py-2 rounded-xl font-semibold text-[#1d3557] hover:bg-[#a8dadc] transition-colors">VER DETALLES ▼</button>
                    <div class="accordion-content">
                        <div class="py-4 px-2 text-gray-600 text-xs space-y-3">
                            <p><strong>🤝 Vínculo:</strong> Mentorías y formación docente a medida.</p>
                            <p><strong>📩 Consulta:</strong> Coordinar disponibilidad según proyecto escolar.</p>
                        </div>
                    </div>
                </div>
            </div>

        </div>

        <div class="mt-12 text-center">
            <a href="https://forms.gle/rwDH4E9ny6HjjNEY8" target="_blank" class="inline-block bg-[#e63946] hover:bg-[#c1121f] text-white text-xl font-bold py-4 px-10 rounded-full shadow-lg transform hover:scale-105 transition-all">
                ¡INSCRIBIRME AHORA! 🚀
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
