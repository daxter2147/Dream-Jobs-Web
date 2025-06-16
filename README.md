
<html lang="es" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- Chosen Palette: "Cool Slate & Teal" - A modern, professional palette using a light slate gray background, dark text for readability, and a vibrant teal/cyan as the primary accent for calls-to-action and highlights. This combination feels trustworthy, technological, and clean. -->
    <!-- Application Structure Plan: The SPA is structured as a narrative journey to build trust and guide two key user types (Companies and Candidates). It starts with a strong Value Proposition (Hero), explains the 'Why' (Benefits) and 'How' (Process), provides data-driven proof ('Success Metrics' Dashboard), builds social proof (Testimonials), offers a tangible tool (AI Interview Prep), and ends with a clear final Call to Action. This structure directly translates the report's recommendations on quantifying value, being transparent, and building credibility, creating a flow that is more persuasive than a simple information page. -->
    <!-- Visualization & Content Choices: 
        - Report Info: Key recruitment metrics (Time to Hire, Retention, Cost Savings). Goal: Demonstrate efficiency and value. Viz/Method: Interactive Bar Chart (Chart.js) and dynamic stat cards. Interaction: Filter chart by industry to show specialized expertise. Justification: Visualizing data makes the agency's performance tangible and trustworthy. Library: Chart.js.
        - Report Info: Importance of a clear, transparent methodology. Goal: Build client trust. Viz/Method: Numbered, visual step-by-step process diagram created with HTML/Tailwind. Interaction: Simple, clear visual flow. Justification: De-mystifies the recruitment process, addressing a key client anxiety identified in the report. Library: N/A (HTML/CSS).
        - Report Info: Need for social proof. Goal: Establish credibility. Viz/Method: Card-based testimonial section. Interaction: Separate tabs/filters for client and candidate testimonials. Justification: Shows success from both perspectives, reinforcing the agency's value proposition. Library: N/A (HTML/CSS).
        - Report Info: Gemini API for value-add. Goal: Engage candidates. Viz/Method: AI-powered question generator. Interaction: User input generates tailored content. Justification: Provides a direct, useful interactive tool that enhances candidate experience. Library: N/A (Fetch API).
    -->
    <!-- CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. -->
    <title>Dream Jobs - Conectamos Talento Excepcional con Empresas Líderes</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8fafc; /* slate-50 */
        }
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
            height: 350px;
            max-height: 400px;
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 400px;
            }
        }
    </style>
</head>
<body class="text-slate-700">

    <!-- Header & Navigation -->
    <header id="header" class="bg-white/80 backdrop-blur-md sticky top-0 z-50 shadow-sm">
        <nav class="container mx-auto px-6 py-4 flex justify-between items-center">
            <a href="#" class="text-2xl font-bold text-slate-800">Dream <span class="text-teal-600">Jobs</span></a>
            <div class="hidden md:flex items-center space-x-6">
                <a href="#porque-elegirnos" class="hover:text-teal-600 transition-colors">Por Qué Elegirnos</a>
                <a href="#proceso" class="hover:text-teal-600 transition-colors">Nuestro Proceso</a>
                <a href="#metricas" class="hover:text-teal-600 transition-colors">Métricas</a>
                <a href="#testimonios" class="hover:text-teal-600 transition-colors">Testimonios</a>
            </div>
            <a href="#unete" class="hidden md:block bg-teal-600 text-white font-semibold px-5 py-2 rounded-lg hover:bg-teal-700 transition-all">Contactar</a>
            <button id="mobile-menu-btn" class="md:hidden text-slate-700">
                <span class="text-2xl">☰</span>
            </button>
        </nav>
        <div id="mobile-menu" class="hidden md:hidden bg-white">
            <a href="#porque-elegirnos" class="block py-2 px-6 text-center hover:bg-slate-100">Por Qué Elegirnos</a>
            <a href="#proceso" class="block py-2 px-6 text-center hover:bg-slate-100">Nuestro Proceso</a>
            <a href="#metricas" class="block py-2 px-6 text-center hover:bg-slate-100">Métricas</a>
            <a href="#testimonios" class="block py-2 px-6 text-center hover:bg-slate-100">Testimonios</a>
            <a href="#unete" class="block py-3 px-6 text-center bg-teal-600 text-white font-semibold">Contactar</a>
        </div>
    </header>

    <main>
        <!-- Hero Section -->
        <section id="hero" class="py-20 md:py-32 bg-slate-100">
            <div class="container mx-auto px-6 text-center">
                <h1 class="text-4xl md:text-6xl font-extrabold text-slate-800 mb-4">Conectamos Talento Excepcional con Empresas Líderes</h1>
                <p class="text-lg md:text-xl text-slate-600 max-w-3xl mx-auto mb-8">Soluciones de reclutamiento a medida para roles remotos en LATAM. Eficiencia, calidad y ahorro de costos en un solo lugar.</p>
                <div class="flex flex-col sm:flex-row justify-center gap-4">
                    <a href="#unete" class="bg-teal-600 text-white font-bold py-3 px-8 rounded-lg text-lg hover:bg-teal-700 transition-all transform hover:scale-105">Busco Talento</a>
                    <a href="#unete" class="bg-white text-teal-600 font-bold py-3 px-8 rounded-lg text-lg border-2 border-teal-600 hover:bg-teal-50 transition-all transform hover:scale-105">Busco Empleo</a>
                </div>
            </div>
        </section>

        <!-- Por Qué Elegirnos Section -->
        <section id="porque-elegirnos" class="py-16 md:py-24">
            <div class="container mx-auto px-6">
                <div class="text-center mb-12">
                    <h2 class="text-3xl md:text-4xl font-bold text-slate-800">Más que Reclutamiento, una Alianza Estratégica</h2>
                    <p class="mt-4 text-lg text-slate-600 max-w-2xl mx-auto">Nuestro enfoque se basa en tres pilares que garantizan el éxito de cada contratación.</p>
                </div>
                <div class="grid md:grid-cols-3 gap-8">
                    <div class="bg-white p-8 rounded-xl shadow-lg border border-slate-200 text-center hover:shadow-2xl hover:-translate-y-2 transition-all">
                        <div class="text-5xl mb-4 text-teal-600">⏱️</div>
                        <h3 class="text-2xl font-bold mb-2 text-slate-800">Tiempo Récord</h3>
                        <p class="text-slate-600">Cubrimos tus vacantes en un promedio de 14 días, un 40% más rápido que el estándar de la industria, para que tu equipo no pierda el ritmo.</p>
                    </div>
                    <div class="bg-white p-8 rounded-xl shadow-lg border border-slate-200 text-center hover:shadow-2xl hover:-translate-y-2 transition-all">
                        <div class="text-5xl mb-4 text-teal-600">🏆</div>
                        <h3 class="text-2xl font-bold mb-2 text-slate-800">Talento Verificado</h3>
                        <p class="text-slate-600">Nuestro riguroso proceso de vetting asegura una tasa de retención del 96%. Solo te presentamos al 3% más destacado de los candidatos.</p>
                    </div>
                    <div class="bg-white p-8 rounded-xl shadow-lg border border-slate-200 text-center hover:shadow-2xl hover:-translate-y-2 transition-all">
                        <div class="text-5xl mb-4 text-teal-600">💰</div>
                        <h3 class="text-2xl font-bold mb-2 text-slate-800">Ahorro Inteligente</h3>
                        <p class="text-slate-600">Reduce tus costos de contratación hasta en un 50% al acceder a nuestro pool de talento en LATAM, sin sacrificar la calidad.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Nuestro Proceso Section -->
        <section id="proceso" class="py-16 md:py-24 bg-slate-100">
            <div class="container mx-auto px-6">
                <div class="text-center mb-12">
                    <h2 class="text-3xl md:text-4xl font-bold text-slate-800">Nuestro Proceso Transparente y Eficaz</h2>
                    <p class="mt-4 text-lg text-slate-600 max-w-2xl mx-auto">Construimos confianza a través de una metodología clara que te acompaña en cada paso.</p>
                </div>
                <div class="relative">
                    <div class="hidden md:block absolute top-1/2 left-0 w-full h-0.5 bg-teal-300 -translate-y-1/2"></div>
                    <div class="grid md:grid-cols-4 gap-8 text-center relative">
                        <div class="flex flex-col items-center">
                            <div class="bg-teal-600 text-white w-16 h-16 rounded-full flex items-center justify-center text-2xl font-bold mb-4 z-10">1</div>
                            <h3 class="text-xl font-semibold mb-2 text-slate-800">Análisis y Definición</h3>
                            <p class="text-slate-600">Comprendemos a fondo tus necesidades, la cultura de tu empresa y los requisitos del rol.</p>
                        </div>
                        <div class="flex flex-col items-center">
                            <div class="bg-teal-600 text-white w-16 h-16 rounded-full flex items-center justify-center text-2xl font-bold mb-4 z-10">2</div>
                            <h3 class="text-xl font-semibold mb-2 text-slate-800">Búsqueda y Vetting</h3>
                            <p class="text-slate-600">Identificamos y evaluamos rigurosamente candidatos a través de pruebas técnicas y de habilidades blandas.</p>
                        </div>
                        <div class="flex flex-col items-center">
                            <div class="bg-teal-600 text-white w-16 h-16 rounded-full flex items-center justify-center text-2xl font-bold mb-4 z-10">3</div>
                            <h3 class="text-xl font-semibold mb-2 text-slate-800">Presentación y Entrevistas</h3>
                            <p class="text-slate-600">Te presentamos una selección curada de los mejores perfiles para que los entrevistes.</p>
                        </div>
                        <div class="flex flex-col items-center">
                            <div class="bg-teal-600 text-white w-16 h-16 rounded-full flex items-center justify-center text-2xl font-bold mb-4 z-10">4</div>
                            <h3 class="text-xl font-semibold mb-2 text-slate-800">Contratación y Soporte</h3>
                            <p class="text-slate-600">Te asistimos en la oferta y el onboarding, asegurando una integración exitosa y con garantía de reemplazo.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- Métricas de Éxito Section -->
        <section id="metricas" class="py-16 md:py-24">
            <div class="container mx-auto px-6">
                <div class="text-center mb-12">
                    <h2 class="text-3xl md:text-4xl font-bold text-slate-800">Resultados que Hablan por Sí Mismos</h2>
                    <p class="mt-4 text-lg text-slate-600 max-w-2xl mx-auto">Explora nuestras métricas de rendimiento y descubre por qué somos el socio de reclutamiento que necesitas.</p>
                </div>
                <div class="bg-white p-6 md:p-8 rounded-xl shadow-lg border border-slate-200">
                    <div class="mb-6 flex justify-center">
                        <div class="flex items-center space-x-2">
                             <label for="industry-filter" class="font-semibold">Filtrar por Industria:</label>
                             <select id="industry-filter" class="p-2 rounded-md border border-slate-300 focus:ring-teal-500 focus:border-teal-500">
                                 <option value="all" selected>Todas</option>
                                 <option value="tech">Tecnología y TI</option>
                                 <option value="sales">Ventas y Marketing</option>
                                 <option value="finance">Finanzas y Contabilidad</option>
                             </select>
                        </div>
                    </div>
                     <div class="chart-container">
                        <canvas id="timeToHireChart"></canvas>
                    </div>
                </div>
            </div>
        </section>

        <!-- Testimonios Section -->
        <section id="testimonios" class="py-16 md:py-24 bg-slate-100">
            <div class="container mx-auto px-6">
                <div class="text-center mb-12">
                    <h2 class="text-3xl md:text-4xl font-bold text-slate-800">La Voz de Nuestros Clientes y Candidatos</h2>
                    <p class="mt-4 text-lg text-slate-600 max-w-2xl mx-auto">La confianza es nuestro mayor activo. Esto es lo que dicen de nosotros.</p>
                </div>
                <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                    <div class="bg-white p-8 rounded-xl shadow-lg border border-slate-200">
                        <p class="text-slate-600 mb-6">"El proceso fue increíblemente rápido y eficiente. Dream Jobs entendió nuestras necesidades a la perfección y nos presentó candidatos de altísima calidad en menos de dos semanas. ¡Impresionante!"</p>
                        <div class="flex items-center">
                            <div class="w-12 h-12 rounded-full bg-teal-100 flex items-center justify-center font-bold text-teal-700 text-lg mr-4">AC</div>
                            <div>
                                <p class="font-bold text-slate-800">Ana C., CEO</p>
                                <p class="text-sm text-slate-500">TechCorp S.A.</p>
                            </div>
                        </div>
                    </div>
                    <div class="bg-white p-8 rounded-xl shadow-lg border border-slate-200">
                        <p class="text-slate-600 mb-6">"Como candidato, me sentí acompañado en todo momento. Me prepararon para la entrevista y encontré un puesto que se ajusta perfectamente a mis habilidades y expectativas. ¡Gracias Dream Jobs!"</p>
                        <div class="flex items-center">
                            <div class="w-12 h-12 rounded-full bg-indigo-100 flex items-center justify-center font-bold text-indigo-700 text-lg mr-4">JP</div>
                             <div>
                                <p class="font-bold text-slate-800">Juan Pérez</p>
                                <p class="text-sm text-slate-500">Desarrollador Senior</p>
                            </div>
                        </div>
                    </div>
                     <div class="bg-white p-8 rounded-xl shadow-lg border border-slate-200 md:col-span-2 lg:col-span-1">
                        <p class="text-slate-600 mb-6">"Redujimos nuestro costo por contratación en un 35% y mejoramos la calidad de los nuevos ingresos. Su modelo de reclutamiento remoto es simplemente superior."</p>
                        <div class="flex items-center">
                            <div class="w-12 h-12 rounded-full bg-rose-100 flex items-center justify-center font-bold text-rose-700 text-lg mr-4">MG</div>
                             <div>
                                <p class="font-bold text-slate-800">Mariela G.</p>
                                <p class="text-sm text-slate-500">Directora de RRHH, Finanzas Global</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- AI Interview Prep Section -->
        <section id="ai-prep" class="py-16 md:py-24">
            <div class="container mx-auto px-6">
                 <div class="bg-white p-6 md:p-8 rounded-xl shadow-2xl border-2 border-teal-500 flex flex-col md:flex-row items-center gap-8">
                    <div class="md:w-1/2">
                        <h2 class="text-3xl md:text-4xl font-bold text-slate-800 mb-4">Prepárate para el Éxito con IA</h2>
                        <p class="text-lg text-slate-600 mb-6">Nuestra herramienta de IA, impulsada por Gemini, te ayuda a generar preguntas de entrevista personalizadas para que llegues con total confianza.</p>
                        <textarea id="interview-context" class="w-full p-3 rounded-md border border-slate-300 focus:ring-teal-500 focus:border-teal-500 resize-y mb-4" rows="3" placeholder="Ej: Tengo 3 años de experiencia en ventas B2B y hablo inglés fluido."></textarea>
                        <button id="generate-questions-btn" class="w-full bg-teal-600 hover:bg-teal-700 text-white font-bold py-3 px-6 rounded-lg text-lg transition-all duration-300 flex items-center justify-center">
                            Generar Preguntas 🧠
                        </button>
                    </div>
                    <div class="md:w-1/2 w-full">
                        <div id="loading-spinner" class="mt-4 text-center text-teal-600 hidden">
                            <div class="animate-spin rounded-full h-8 w-8 border-b-2 border-teal-600 mx-auto"></div>
                            <p class="mt-2">Generando preguntas...</p>
                        </div>
                        <div id="interview-questions-output" class="mt-4 p-4 bg-slate-50 rounded-lg border border-slate-200 h-64 overflow-y-auto hidden">
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Final CTA Section -->
        <section id="unete" class="py-16 md:py-24 bg-slate-800 text-white">
            <div class="container mx-auto px-6 text-center">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">¿Listo para Construir tu Equipo Soñado o Encontrar tu Trabajo Ideal?</h2>
                <p class="text-lg text-slate-300 max-w-2xl mx-auto mb-8">Hablemos sobre cómo podemos ayudarte a alcanzar tus objetivos. La consulta inicial es sin compromiso.</p>
                <a href="#" class="bg-teal-500 hover:bg-teal-400 text-white font-bold py-4 px-10 rounded-lg text-xl transition-all duration-300 transform hover:scale-105">Comienza Ahora</a>
            </div>
        </section>
    </main>
    
    <!-- Footer -->
    <footer class="bg-slate-900 text-slate-400 py-8">
        <div class="container mx-auto px-6 text-center">
            <p>&copy; 2024 Dream Jobs. Todos los derechos reservados.</p>
            <p class="text-sm mt-2">Conectando talento y oportunidades en toda LATAM.</p>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            // Mobile Menu Toggle
            const mobileMenuBtn = document.getElementById('mobile-menu-btn');
            const mobileMenu = document.getElementById('mobile-menu');
            mobileMenuBtn.addEventListener('click', () => {
                mobileMenu.classList.toggle('hidden');
            });

            // Smooth scrolling for nav links
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function (e) {
                    e.preventDefault();
                    const targetId = this.getAttribute('href');
                    const targetElement = document.querySelector(targetId);
                    if (targetElement) {
                        targetElement.scrollIntoView({
                            behavior: 'smooth'
                        });
                        if (mobileMenu.classList.contains('hidden') === false) {
                           mobileMenu.classList.add('hidden');
                        }
                    }
                });
            });

            // Chart.js Logic
            const ctx = document.getElementById('timeToHireChart').getContext('2d');
            let timeToHireChart;

            const chartData = {
                all: {
                    labels: ['Nuestro Promedio', 'Promedio Industria'],
                    data: [14, 24]
                },
                tech: {
                    labels: ['Nuestro Promedio (Tech)', 'Promedio Industria (Tech)'],
                    data: [18, 30]
                },
                sales: {
                    labels: ['Nuestro Promedio (Ventas)', 'Promedio Industria (Ventas)'],
                    data: [12, 22]
                },
                finance: {
                    labels: ['Nuestro Promedio (Finanzas)', 'Promedio Industria (Finanzas)'],
                    data: [16, 25]
                }
            };
            
            function createOrUpdateChart(data) {
                if (timeToHireChart) {
                    timeToHireChart.destroy();
                }
                
                timeToHireChart = new Chart(ctx, {
                    type: 'bar',
                    data: {
                        labels: data.labels,
                        datasets: [{
                            label: 'Días para Contratar',
                            data: data.data,
                            backgroundColor: [
                                'rgba(13, 148, 136, 0.7)', // teal-600
                                'rgba(100, 116, 139, 0.5)' // slate-500
                            ],
                            borderColor: [
                                'rgba(13, 148, 136, 1)',
                                'rgba(100, 116, 139, 1)'
                            ],
                            borderWidth: 1
                        }]
                    },
                    options: {
                        responsive: true,
                        maintainAspectRatio: false,
                        plugins: {
                            legend: {
                                display: false
                            },
                            tooltip: {
                                callbacks: {
                                    label: function(context) {
                                        return `${context.dataset.label}: ${context.raw} días`;
                                    }
                                }
                            },
                            title: {
                                display: true,
                                text: 'Comparativa de Tiempo para Contratar (en días)',
                                font: {
                                    size: 16
                                },
                                padding: {
                                    top: 10,
                                    bottom: 20
                                }
                            }
                        },
                        scales: {
                            y: {
                                beginAtZero: true,
                                title: {
                                    display: true,
                                    text: 'Días'
                                }
                            }
                        }
                    }
                });
            }

            const industryFilter = document.getElementById('industry-filter');
            industryFilter.addEventListener('change', (e) => {
                const selectedIndustry = e.target.value;
                createOrUpdateChart(chartData[selectedIndustry]);
            });

            createOrUpdateChart(chartData.all);

            // Gemini API integration
            const generateQuestionsBtn = document.getElementById('generate-questions-btn');
            const interviewContextInput = document.getElementById('interview-context');
            const interviewQuestionsOutput = document.getElementById('interview-questions-output');
            const loadingSpinner = document.getElementById('loading-spinner');

            const jobDescription = `
                Oportunidad de Empleo: Vendedores Remotos
                Estamos contratando vendedores en LATAM y Centroamérica.
                Ofrecemos: Capacitación pagada, Trabajo remoto, Salario en dólares, Pagos quincenales, Pagos a través de Binance, Salario comisional de $500 USD (con posibilidad de aumentar), Horario full time y part time.
                Requisitos indispensables: Nivel de inglés intermedio, Laptop o PC de 5ta generación o superior (mínimo 8GB de RAM), Conexión a internet estable, Tener entre 18 a 35 años.
            `;

            generateQuestionsBtn.addEventListener('click', async () => {
                const userContext = interviewContextInput.value.trim();
                interviewQuestionsOutput.innerHTML = '';
                interviewQuestionsOutput.classList.add('hidden');
                loadingSpinner.classList.remove('hidden');

                const prompt = \`Actúa como un coach de entrevistas experto. Genera 5 preguntas de entrevista clave para un puesto de vendedor remoto, basándote en esta descripción: \${jobDescription}. \${userContext ? \`Considera también esta información adicional del candidato: "\${userContext}".\` : ''} Las preguntas deben ser perspicaces, estar en español y presentadas como una lista con viñetas.\`;

                let chatHistory = [{ role: "user", parts: [{ text: prompt }] }];
                const payload = { contents: chatHistory };
                const apiKey = "";
                const apiUrl = \`https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent?key=\${apiKey}\`;

                try {
                    const response = await fetch(apiUrl, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify(payload)
                    });
                    const result = await response.json();
                    
                    if (result.candidates && result.candidates[0].content.parts) {
                        const text = result.candidates[0].content.parts[0].text;
                        const formattedText = text.replace(/\\*\\s?/g, '').replace(/\\n/g, '<br>');
                        interviewQuestionsOutput.innerHTML = \`<h3 class="font-semibold text-lg mb-2 text-slate-800">Preguntas Sugeridas:</h3><ul class="list-disc list-inside space-y-2">\${formattedText.split('<br>').map(q => q.trim() ? \`<li>\${q.replace(/^- /, '')}</li>\` : '').join('')}</ul>\`;
                        interviewQuestionsOutput.classList.remove('hidden');
                    } else {
                        throw new Error("Respuesta inesperada de la API.");
                    }
                } catch (error) {
                    interviewQuestionsOutput.innerHTML = \`<p class="text-red-500">Error al generar preguntas. Por favor, inténtalo de nuevo.</p>\`;
                    interviewQuestionsOutput.classList.remove('hidden');
                    console.error("Error:", error);
                } finally {
                    loadingSpinner.classList.add('hidden');
                }
            });
        });
    </script>
</body>
</html>
