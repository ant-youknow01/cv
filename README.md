<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Infographic CV | Antonio Buys</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700;900&display=swap" rel="stylesheet">
    <!-- Chosen Palette: Energetic & Playful -->
    <!-- Application Structure Plan: A top-down narrative flow telling a story. It starts with a strong headline, moves to a "big number" stat (3+ years experience), then visually breaks down skills into categories. The core is a chronological, visual timeline of career progression at YOUKNOW, followed by a grid of certifications. This linear, story-driven structure is chosen to guide the user through the career journey logically, making it easy to digest the transition from music to a successful tech career. -->
    <!-- Visualization & Content Choices: 
    - Key Stat: Report Info -> 3+ years experience -> Goal -> Inform -> Viz/Presentation -> Single Big Number -> Justification -> Immediately establishes credibility and experience level. Method: HTML/Tailwind.
    - Skills Breakdown: Report Info -> Skills list -> Goal -> Compare/Organize -> Viz/Presentation -> Donut Chart -> Justification -> Visually segments diverse skills into understandable categories (Technical, Core, Soft), showing a well-rounded profile. Library: Chart.js.
    - Career Timeline: Report Info -> Work History at YOUKNOW -> Goal -> Show Change/Process -> Viz/Presentation -> Styled HTML/CSS Timeline -> Justification -> Clearly illustrates career progression and increasing responsibility over time in a visually engaging way. Method: HTML/Tailwind.
    - Certifications: Report Info -> Licenses & Certs -> Goal -> Organize/Inform -> Viz/Presentation -> Icon Grid -> Justification -> Presents a large number of certifications in a compact, scannable format using Unicode icons for visual appeal. Method: HTML/Tailwind. -->
    <!-- CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. -->
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #0F172A; /* slate-900 */
            color: #F8FAFC; /* slate-50 */
        }
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 400px;
            margin-left: auto;
            margin-right: auto;
            height: 300px;
            max-height: 400px;
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 350px;
            }
        }
        .timeline::before {
            content: '';
            position: absolute;
            left: 50%;
            transform: translateX(-50%);
            top: 0;
            width: 4px;
            height: 100%;
            background-color: #334155; /* slate-700 */
        }
        .timeline-item-dot {
            position: absolute;
            left: 50%;
            transform: translateX(-50%);
            width: 24px;
            height: 24px;
            border-radius: 50%;
            background-color: #F43F5E; /* rose-500 */
            border: 4px solid #0F172A; /* slate-900 */
        }
    </style>
</head>
<body class="antialiased">

    <div class="container mx-auto p-4 md:p-8 max-w-5xl">

        <header class="text-center my-12">
            <h1 class="text-5xl md:text-7xl font-black tracking-tighter text-white">ANTONIO BUYS</h1>
            <p class="mt-4 text-2xl md:text-3xl font-bold text-rose-500">Solutions Consultant | MarTech Specialist</p>
        </header>

        <section class="my-16 bg-slate-800 p-8 rounded-2xl shadow-2xl">
            <div class="grid md:grid-cols-2 gap-8 items-center">
                <div class="text-center">
                    <p class="text-2xl text-slate-300">A highly effective and certified Solutions Consultant transforming how African brands leverage marketing technology.</p>
                </div>
                <div class="text-center bg-rose-500 p-8 rounded-xl">
                    <p class="text-8xl font-black text-white">3+</p>
                    <p class="text-2xl font-bold text-rose-100">Years of Experience</p>
                </div>
            </div>
        </section>

        <section class="my-16 text-center">
            <h2 class="text-4xl font-bold mb-4">A Blend of Expertise</h2>
            <p class="max-w-3xl mx-auto mt-8 text-slate-300 text-2xl leading-relaxed">My skill set is a made up of a combination of deep technical knowledge, strategic consulting competencies, and essential soft skills for driving client success.</p>
            <div class="chart-container">
                <canvas id="skillsChart"></canvas>
            </div>
            <p class="max-w-3xl mx-auto mt-8 text-slate-300 text-2xl leading-relaxed">
                My technical expertise spans a wide range of marketing technologies, including Braze, Domo, and Amplitude, supported by key certifications in each. My competencies in Agile Project Management and software consulting enable me to strategically guide projects from concept to completion. Finally, I have developed soft skills, such as problem-solving and communication, which are crucial for fostering strong client relationships and adapting to dynamic challenges within the industry.
            </p>
        </section>

        <section class="my-16">
            <h2 class="text-4xl font-bold text-center mb-12">Career Progression at YOUKNOW</h2>
            <div class="relative timeline py-8">
                
                <div class="relative md:flex my-8">
                    <div class="timeline-item-dot mt-1 hidden md:block"></div>
                    <div class="md:w-1/2 md:pr-12"></div>
                    <div class="md:w-1/2 md:pl-12">
                        <div class="bg-slate-800 p-6 rounded-xl shadow-lg">
                            <p class="text-xl text-rose-400 font-bold">NOV 2024 - PRESENT</p>
                            <h3 class="text-2xl font-bold text-white">Solutions Consultant</h3>
                            <p class="mt-2 text-xl text-slate-300">Spearheading implementations, delivering bespoke solutions, and providing strategic guidance to empower clients.</p>
                        </div>
                    </div>
                </div>

                <div class="relative md:flex my-8">
                    <div class="timeline-item-dot mt-1 hidden md:block"></div>
                    <div class="md:w-1/2 md:pr-12">
                         <div class="bg-slate-800 p-6 rounded-xl shadow-lg text-right md:text-left">
                            <p class="text-xl text-rose-400 font-bold">MAR 2023 - NOV 2024</p>
                            <h3 class="text-2xl font-bold text-white">Onboarding & Platform Specialist</h3>
                            <p class="mt-2 text-xl text-slate-300">Managed end-to-end client onboarding and served as a key point of contact for technical inquiries.</p>
                        </div>
                    </div>
                    <div class="md:w-1/2 md:pl-12"></div>
                </div>

                <div class="relative md:flex my-8">
                    <div class="timeline-item-dot mt-1 hidden md:block"></div>
                    <div class="md:w-1/2 md:pr-12"></div>
                    <div class="md:w-1/2 md:pl-12">
                        <div class="bg-slate-800 p-6 rounded-xl shadow-lg">
                            <p class="text-xl text-rose-400 font-bold">APR 2022 - MAR 2023</p>
                            <h3 class="text-2xl font-bold text-white">Technical Support Specialist</h3>
                            <p class="mt-2 text-xl text-slate-300">Provided expert technical support, diagnosing and resolving a wide range of customer issues efficiently.</p>
                        </div>
                    </div>
                </div>

            </div>
        </section>

        <section class="my-16">
            <h2 class="text-4xl font-bold text-center mb-4">Certified & Proficient</h2>
            <p class="max-w-2xl mx-auto text-center text-2xl text-slate-300 mb-12">Committed to continuous learning, holding numerous certifications across the MarTech ecosystem.</p>
            <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4 text-center">
                <div class="bg-slate-800 p-4 rounded-lg"><span class="text-3xl mr-2">🔧</span> Braze</div>
                <div class="bg-slate-800 p-4 rounded-lg"><span class="text-3xl mr-2">📊</span> Domo</div>
                <div class="bg-slate-800 p-4 rounded-lg"><span class="text-3xl mr-2">📈</span> Amplitude</div>
                <div class="bg-slate-800 p-4 rounded-lg"><span class="text-3xl mr-2">🔔</span> Mixpanel</div>
                <div class="bg-slate-800 p-4 rounded-lg"><span class="text-3xl mr-2">🔗</span> mParticle</div>
                <div class="bg-slate-800 p-4 rounded-lg"><span class="text-3xl mr-2">🦉</span> Hootsuite</div>
                <div class="bg-slate-800 p-4 rounded-lg"><span class="text-3xl mr-2">🛰️</span> Postman API</div>
                <div class="bg-slate-800 p-4 rounded-lg"><span class="text-3xl mr-2">🌐</span> Google Analytics</div>
                <div class="bg-slate-800 p-4 rounded-lg"><span class="text-3xl mr-2">🔍</span> Brandwatch</div>
                <div class="bg-slate-800 p-4 rounded-lg"><span class="text-3xl mr-2">⚙️</span> HubSpot</div>
                <div class="bg-slate-800 p-4 rounded-lg"><span class="text-3xl mr-2">🏃</span> Agile PM</div>
                <div class="bg-slate-800 p-4 rounded-lg"><span class="text-3xl mr-2">💡</span> Digital Strategist</div>
            </div>
        </section>

        <footer class="text-center mt-16 py-8 border-t border-slate-700">
            <p class="text-slate-400">Infographic CV for Antonio Buys | Data-driven, client-focused, and ready to innovate.</p>
        </footer>

    </div>

    <script>
        const skillsChartCtx = document.getElementById('skillsChart').getContext('2d');
        const skillsChart = new Chart(skillsChartCtx, {
            type: 'doughnut',
            data: {
                labels: ['Technical Expertise', 'Soft Skills', 'Core Competencies'],
                datasets: [{
                    label: 'Skills Breakdown',
                    data: [11, 6, 5],
                    backgroundColor: [
                        '#F43F5E', // rose-500
                        '#FBBF24', // amber-400
                        '#38BDF8'  // sky-400
                    ],
                    borderColor: '#0F172A',
                    borderWidth: 4,
                    hoverOffset: 8
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                cutout: '60%',
                plugins: {
                    legend: {
                        position: 'bottom',
                        labels: {
                            color: '#CBD5E1', // slate-300
                            font: {
                                size: 14,
                                family: 'Inter'
                            }
                        }
                    },
                    tooltip: {
                        callbacks: {
                            title: function(tooltipItems) {
                                const item = tooltipItems[0];
                                let label = item.chart.data.labels[item.dataIndex];
                                if (Array.isArray(label)) {
                                  return label.join(' ');
                                } else {
                                  return label;
                                }
                            }
                        }
                    }
                }
            }
        });
    </script>

</body>
</html>
