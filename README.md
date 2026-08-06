<!DOCTYPE html>
<html lang="zh-CN" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Allie Woon — Professional Portfolio</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Noto Sans SC (Source Han Sans) and Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600&family=Noto+Sans+SC:wght@100;200;300;400;500;700&display=swap" rel="stylesheet">
    <!-- FontAwesome icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Noto Sans SC', 'Inter', 'sans-serif'],
                    },
                    colors: {
                        brand: {
                            pink: '#ff8da1',
                            pinkLight: 'rgba(255, 141, 161, 0.12)',
                            bg: '#fbfbfb',
                            dark: '#121212',
                            muted: '#6e6e73'
                        }
                    }
                }
            }
        }
    </script>
    
    <style>
        body {
            cursor: none; /* Hide standard cursor to enable elegant pink glass cursor */
            background-color: #fbfbfb;
        }
        a, button, select, input, textarea, [role="button"], .interactive-node {
            cursor: none;
        }
        /* Custom scrollbar matching premium Mac aesthetic */
        ::-webkit-scrollbar {
            width: 5px;
            height: 5px;
        }
        ::-webkit-scrollbar-track {
            background: #f5f5f7;
        }
        ::-webkit-scrollbar-thumb {
            background: #d2d2d7;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #86868b;
        }
        .no-scrollbar::-webkit-scrollbar {
            display: none;
        }
        .no-scrollbar {
            -ms-overflow-style: none;
            scrollbar-width: none;
        }
        .delay-1 { transition-delay: 40ms; }
        .delay-2 { transition-delay: 80ms; }
        .delay-3 { transition-delay: 120ms; }
        .delay-4 { transition-delay: 160ms; }
        .delay-5 { transition-delay: 200ms; }
    </style>
</head>
<body class="font-sans font-light text-brand-dark antialiased overflow-x-hidden">

    <div id="cursor-dot" class="fixed top-0 left-0 w-2.5 h-2.5 bg-pink-500 rounded-full pointer-events-none z-[9999] -translate-x-1/2 -translate-y-1/2 transition-transform duration-75 ease-out"></div>
    <div id="cursor-outline" class="fixed top-0 left-0 w-11 h-11 rounded-full border border-pink-400/50 bg-pink-300/10 backdrop-blur-[3px] pointer-events-none z-[9998] -translate-x-1/2 -translate-y-1/2 transition-all duration-300 ease-out"></div>

    <nav class="fixed top-0 left-0 w-full z-50 px-8 py-6 flex justify-between items-center mix-blend-difference">
        <div class="text-xs uppercase tracking-[0.3em] font-light text-white">
            <a href="#home" class="interactive-node">ALLIE.WOON</a>
        </div>
        <div class="text-xs uppercase tracking-[0.2em] font-light text-white hidden md:block text-right">
            Healthcare, Clinical & Commercial Operations Portfolio
        </div>
    </nav>

    <section id="home" class="min-h-screen w-full flex flex-col justify-center items-center px-6 relative bg-brand-bg">
        <div class="absolute inset-0 grid grid-cols-4 pointer-events-none border-x border-gray-100">
            <div class="border-r border-gray-100/50"></div>
            <div class="border-r border-gray-100/50"></div>
            <div class="border-r border-gray-100/50"></div>
        </div>

        <div class="z-10 text-center max-w-4xl px-4 select-none">
            <p class="text-xs uppercase tracking-[0.4em] text-brand-muted mb-6 font-light">
                Monash University — Pharmaceutical Science
            </p>
            
            <div class="relative inline-block group" id="directory-trigger">
                <h1 class="text-4xl md:text-7xl font-light tracking-tight text-brand-dark transition-all duration-500 group-hover:text-pink-500/80 cursor-none py-4 uppercase">
                    INDEX <span class="font-extralight text-gray-300 group-hover:text-pink-300 transition-colors">/</span> DIRECTORY
                </h1>
                <div class="text-xs text-brand-muted mt-2 tracking-[0.15em] uppercase font-light opacity-60 group-hover:opacity-100 transition-opacity">
                    ( hover cursor here to explore )
                </div>

                <!-- Dropdown items with optimized directory titles -->
                <div id="directory-dropdown" class="absolute top-[110%] left-1/2 -translate-x-1/2 w-72 md:w-80 bg-white/70 backdrop-blur-md border border-white/40 shadow-[0_15px_40px_rgba(0,0,0,0.04)] rounded-2xl py-6 px-4 flex flex-col gap-3 opacity-0 pointer-events-none scale-95 transition-all duration-500 ease-out z-20">
                    <a href="#about-me" class="directory-item group/item flex justify-between items-center py-2 px-4 rounded-lg hover:bg-white/90 transition-all duration-300 opacity-0 -translate-y-2 delay-1">
                        <span class="text-xs text-brand-muted group-hover/item:text-pink-500 transition-colors">01 /</span>
                        <span class="text-xs font-light tracking-[0.2em] uppercase text-brand-dark group-hover/item:text-brand-dark transition-colors">about me</span>
                        <i class="fa-solid fa-arrow-right-long text-[10px] text-gray-300 group-hover/item:text-pink-400 group-hover/item:translate-x-1 transition-all"></i>
                    </a>
                    <a href="#skills" class="directory-item group/item flex justify-between items-center py-2 px-4 rounded-lg hover:bg-white/90 transition-all duration-300 opacity-0 -translate-y-2 delay-2">
                        <span class="text-xs text-brand-muted group-hover/item:text-pink-500 transition-colors">02 /</span>
                        <span class="text-xs font-light tracking-[0.2em] uppercase text-brand-dark group-hover/item:text-brand-dark transition-colors">skills</span>
                        <i class="fa-solid fa-arrow-right-long text-[10px] text-gray-300 group-hover/item:text-pink-400 group-hover/item:translate-x-1 transition-all"></i>
                    </a>
                    <a href="#experience" class="directory-item group/item flex justify-between items-center py-2 px-4 rounded-lg hover:bg-white/90 transition-all duration-300 opacity-0 -translate-y-2 delay-3">
                        <span class="text-xs text-brand-muted group-hover/item:text-pink-500 transition-colors">03 /</span>
                        <span class="text-xs font-light tracking-[0.2em] uppercase text-brand-dark group-hover/item:text-brand-dark transition-colors">experience</span>
                        <i class="fa-solid fa-arrow-right-long text-[10px] text-gray-300 group-hover/item:text-pink-400 group-hover/item:translate-x-1 transition-all"></i>
                    </a>
                    <a href="#blueprints" class="directory-item group/item flex justify-between items-center py-2 px-4 rounded-lg hover:bg-white/90 transition-all duration-300 opacity-0 -translate-y-2 delay-4">
                        <span class="text-xs text-brand-muted group-hover/item:text-pink-500 transition-colors">04 /</span>
                        <span class="text-xs font-light tracking-[0.2em] uppercase text-brand-dark group-hover/item:text-brand-dark transition-colors">blueprints</span>
                        <i class="fa-solid fa-arrow-right-long text-[10px] text-gray-300 group-hover/item:text-pink-400 group-hover/item:translate-x-1 transition-all"></i>
                    </a>
                    <a href="#contact-me" class="directory-item group/item flex justify-between items-center py-2 px-4 rounded-lg hover:bg-white/90 transition-all duration-300 opacity-0 -translate-y-2 delay-5">
                        <span class="text-xs text-brand-muted group-hover/item:text-pink-500 transition-colors">05 /</span>
                        <span class="text-xs font-light tracking-[0.2em] uppercase text-brand-dark group-hover/item:text-brand-dark transition-colors">contact me</span>
                        <i class="fa-solid fa-arrow-right-long text-[10px] text-gray-300 group-hover/item:text-pink-400 group-hover/item:translate-x-1 transition-all"></i>
                    </a>
                </div>
            </div>
        </div>

        <div class="absolute bottom-12 left-1/2 -translate-x-1/2 flex flex-col items-center gap-2">
            <span class="text-[9px] uppercase tracking-[0.3em] text-brand-muted font-light">Explore Target Fields</span>
            <div class="w-[1px] h-8 bg-gray-200 relative overflow-hidden">
                <div class="absolute top-0 left-0 w-full h-1/2 bg-pink-400 animate-bounce"></div>
            </div>
        </div>
    </section>

    <section id="about-me" class="min-h-screen py-32 px-6 md:px-12 lg:px-24 bg-white relative flex flex-col justify-center">
        <div class="max-w-7xl mx-auto w-full">
            
            <div class="mb-16">
                <span class="text-xs uppercase tracking-[0.4em] text-pink-400 font-light block mb-2">01 / OVERVIEW</span>
                <h2 class="text-2xl font-light tracking-wide text-brand-dark uppercase">About Me / 个人简介</h2>
                <div class="w-12 h-[1px] bg-pink-200 mt-4"></div>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 lg:gap-16 items-start">
                
                <!-- Left: Aesthetic Portrait Card Placeholder -->
                <div class="lg:col-span-5 w-full flex justify-center">
                    <div class="relative group max-w-sm w-full aspect-[3/4] rounded-2xl overflow-hidden bg-gray-100 border border-gray-100 shadow-sm">
                        <div class="absolute inset-0 flex flex-col items-center justify-center p-8 bg-gradient-to-b from-gray-50 to-neutral-100 text-center">
                            <div class="w-28 h-28 rounded-full border border-pink-100 bg-white/80 backdrop-blur-sm flex items-center justify-center mb-6 shadow-sm overflow-hidden group-hover:border-pink-300 transition-colors duration-500">
                                <i class="fa-solid fa-briefcase-medical text-3xl text-pink-300/80 group-hover:text-pink-400 transition-colors duration-500"></i>
                            </div>
                            <span class="text-sm font-normal tracking-[0.1em] text-brand-dark">ALLIE WOON</span>
                            <span class="text-[10px] text-brand-muted uppercase tracking-[0.15em] mt-1">Woon Zhi Yu</span>
                            <span class="text-[9px] text-pink-400 uppercase tracking-[0.1em] mt-2 bg-pink-50/50 px-3 py-1 rounded-full border border-pink-100">Monash University</span>
                            
                            <div class="absolute bottom-6 left-6 right-6 flex justify-between text-[9px] uppercase tracking-[0.15em] text-gray-400 border-t border-gray-200/50 pt-3">
                                <span>Pharm Science Student</span>
                                <span>Melbourne / Victoria</span>
                            </div>
                        </div>
                        <div class="absolute inset-0 bg-pink-500/5 opacity-0 group-hover:opacity-100 transition-opacity duration-500"></div>
                    </div>
                </div>

                <!-- Right: Education, Profile Statement, Coursework, Languages stacked elegantly -->
                <div class="lg:col-span-7 space-y-8">
                    
                    <!-- Strategic Professional Summary -->
                    <div class="space-y-3">
                        <h3 class="text-xs uppercase tracking-[0.3em] text-brand-muted font-normal">Career Vision / 职业图景</h3>
                        <p class="text-sm text-brand-dark leading-relaxed font-light text-justify">
                            Pharmaceutical Science student at Monash University Malaysia with strong communication and commercial skills interested in healthcare/pharma. Hands-on experience in public relations, technical promotion, and customer operations. Exceptionally positioned to assist healthcare and life sciences employers in <strong>Clinical Operations (CTA/CRC)</strong>, <strong>Medical Device Support</strong>, and <strong>Pharma Commercial Networks</strong>. Bilingual in English and Mandarin, with a proven track record of managing details and engaging diverse clients with commercial confidence.
                        </p>
                    </div>

                    <div class="h-[1px] bg-gray-100"></div>

                    <!-- Education & Languages Grid -->
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                        
                        <!-- Education -->
                        <div class="space-y-3">
                            <h3 class="text-xs uppercase tracking-[0.3em] text-brand-muted font-normal">Education / 教育背景</h3>
                            <div class="group">
                                <div class="text-[11px] text-pink-400 font-light uppercase tracking-[0.15em]">Expected Graduation 2027</div>
                                <div class="text-xs font-normal text-brand-dark">Monash University Malaysia</div>
                                <div class="text-[11px] text-brand-muted uppercase tracking-[0.1em] mt-1">Bachelor of Pharmaceutical Science</div>
                            </div>
                        </div>

                        <!-- Languages (Cleaned to show only high-value professional competencies) -->
                        <div class="space-y-3">
                            <h3 class="text-xs uppercase tracking-[0.3em] text-brand-muted font-normal">Languages / 语言能力</h3>
                            <div class="flex flex-col gap-2.5 text-xs">
                                <div class="flex items-center gap-1.5">
                                    <span class="w-1.5 h-1.5 rounded-full bg-pink-400"></span>
                                    <span class="text-brand-dark font-normal">English <span class="text-[10px] text-brand-muted">(Fluent)</span></span>
                                </div>
                                <div class="flex items-center gap-1.5">
                                    <span class="w-1.5 h-1.5 rounded-full bg-pink-400"></span>
                                    <span class="text-brand-dark font-normal">Mandarin / Chinese <span class="text-[10px] text-brand-muted">(Native)</span></span>
                                </div>
                                <div class="flex items-center gap-1.5">
                                    <span class="w-1.5 h-1.5 rounded-full bg-pink-200"></span>
                                    <span class="text-brand-dark font-light">Cantonese <span class="text-[10px] text-brand-muted">(Conversational)</span></span>
                                </div>
                            </div>
                        </div>

                    </div>

                    <div class="h-[1px] bg-gray-100"></div>

                    <!-- New addition: Relevant Academic Coursework (Reminds recruiters she is a scientist) -->
                    <div class="space-y-3">
                        <h3 class="text-xs uppercase tracking-[0.3em] text-brand-muted font-normal">Relevant Coursework / 相关核心课程</h3>
                        <div class="flex flex-wrap gap-2 pt-1">
                            <span class="text-[10px] bg-neutral-50 border border-neutral-200 text-brand-dark px-3 py-1.5 rounded-full tracking-wider">Pharmacology</span>
                            <span class="text-[10px] bg-neutral-50 border border-neutral-200 text-brand-dark px-3 py-1.5 rounded-full tracking-wider">Drug Discovery</span>
                            <span class="text-[10px] bg-neutral-50 border border-neutral-200 text-brand-dark px-3 py-1.5 rounded-full tracking-wider">Medicinal Chemistry</span>
                            <span class="text-[10px] bg-neutral-50 border border-neutral-200 text-brand-dark px-3 py-1.5 rounded-full tracking-wider">Human Physiology</span>
                            <span class="text-[10px] bg-neutral-50 border border-neutral-200 text-brand-dark px-3 py-1.5 rounded-full tracking-wider">Pharmaceutical Formulation</span>
                        </div>
                    </div>

                </div>

            </div>

        </div>
    </section>

    <section id="skills" class="min-h-screen py-32 px-6 md:px-12 lg:px-24 bg-gray-50/50 relative flex flex-col justify-center overflow-hidden">
        <div class="absolute top-12 left-6 md:left-12 lg:left-24">
            <span class="text-[10px] uppercase tracking-[0.6em] text-brand-muted font-normal">skills</span>
        </div>

        <div class="max-w-7xl mx-auto w-full relative z-10">
            <div class="mb-16 text-center max-w-xl mx-auto">
                <span class="text-xs uppercase tracking-[0.4em] text-pink-400 font-light block mb-2">02 / INTERACTIVE SKILL INSPECTOR</span>
                <h2 class="text-2xl font-light tracking-wide text-brand-dark uppercase">Core Competencies</h2>
                <p class="text-xs text-brand-muted tracking-wider mt-2 font-light">Swipe/scroll or click the grey-transparent glass cards to inspect technical details in the MacBook simulator below.</p>
            </div>

            <div class="relative w-full max-w-4xl mx-auto pt-16">
                
                <!-- Curated, High-value Skill Cards -->
                <div class="absolute -top-6 left-1/2 -translate-x-1/2 w-full max-w-3xl z-20 px-4">
                    <div class="flex gap-4 overflow-x-auto py-4 px-2 no-scrollbar scroll-smooth cursor-grab select-none" id="skills-cards-container">
                        
                        <!-- Card 1 -->
                        <div class="skill-card flex-shrink-0 w-44 md:w-48 p-5 rounded-2xl bg-white/70 backdrop-blur-md border border-white/60 shadow-sm hover:shadow-md hover:-translate-y-1 transition-all duration-300 cursor-none" data-skill-title="Product Education & Promotion" data-skill-desc="Skilled at translating complex scientific, chemical, or formulation parameters into logical user benefits. Experienced performing technical presentations and live demonstrations to engage and convert clients." data-skill-progress="95" data-skill-tag="Product Demonstration">
                            <div class="w-10 h-10 rounded-xl bg-pink-100/40 flex items-center justify-center mb-4">
                                <i class="fa-solid fa-graduation-cap text-pink-400 text-sm"></i>
                            </div>
                            <h3 class="text-xs uppercase tracking-wider font-semibold text-brand-dark mb-1">Product Education</h3>
                            <span class="text-[9px] uppercase tracking-wider text-brand-muted">Clinical Specialist</span>
                        </div>

                        <!-- Card 2 -->
                        <div class="skill-card flex-shrink-0 w-44 md:w-48 p-5 rounded-2xl bg-white/70 backdrop-blur-md border border-white/60 shadow-sm hover:shadow-md hover:-translate-y-1 transition-all duration-300 cursor-none" data-skill-title="Customer Communication" data-skill-desc="Fluent in English and Mandarin with outstanding conversational agility. Adept at handling objections, managing diverse client circles, and setting high-value customer satisfaction standards." data-skill-progress="94" data-skill-tag="Client Engagement">
                            <div class="w-10 h-10 rounded-xl bg-gray-100 flex items-center justify-center mb-4">
                                <i class="fa-solid fa-comments text-pink-400 text-sm"></i>
                            </div>
                            <h3 class="text-xs uppercase tracking-wider font-semibold text-brand-dark mb-1">Customer Comm</h3>
                            <span class="text-[9px] uppercase tracking-wider text-brand-muted">Bilingual Agility</span>
                        </div>

                        <!-- Card 3 -->
                        <div class="skill-card flex-shrink-0 w-44 md:w-48 p-5 rounded-2xl bg-white/70 backdrop-blur-md border border-white/60 shadow-sm hover:shadow-md hover:-translate-y-1 transition-all duration-300 cursor-none" data-skill-title="Sales & Relationship Building" data-skill-desc="Proven face-to-face commercial persuasion. Competent in analyzing client requirements, establishing rapport, POS operations, and organizing promotional campaigns." data-skill-progress="90" data-skill-tag="Pharma Sales">
                            <div class="w-10 h-10 rounded-xl bg-gray-100 flex items-center justify-center mb-4">
                                <i class="fa-solid fa-handshake text-pink-400 text-sm"></i>
                            </div>
                            <h3 class="text-xs uppercase tracking-wider font-semibold text-brand-dark mb-1">Sales & Relations</h3>
                            <span class="text-[9px] uppercase tracking-wider text-brand-muted">Commercial BD</span>
                        </div>

                        <!-- Card 4 -->
                        <div class="skill-card flex-shrink-0 w-44 md:w-48 p-5 rounded-2xl bg-white/70 backdrop-blur-md border border-white/60 shadow-sm hover:shadow-md hover:-translate-y-1 transition-all duration-300 cursor-none" data-skill-title="Scientific Knowledge" data-skill-desc="Strong academic foundations in Pharmacology, Drug Formulation, Medicinal Chemistry, and Human Physiology. Experienced with scientific rigor and standard operating guidelines." data-skill-progress="92" data-skill-tag="Pharmaceutical Science">
                            <div class="w-10 h-10 rounded-xl bg-gray-100 flex items-center justify-center mb-4">
                                <i class="fa-solid fa-flask text-pink-400 text-sm"></i>
                            </div>
                            <h3 class="text-xs uppercase tracking-wider font-semibold text-brand-dark mb-1">Scientific Core</h3>
                            <span class="text-[9px] uppercase tracking-wider text-brand-muted">Clinical Assistant</span>
                        </div>

                        <!-- Card 5 -->
                        <div class="skill-card flex-shrink-0 w-44 md:w-48 p-5 rounded-2xl bg-white/70 backdrop-blur-md border border-white/60 shadow-sm hover:shadow-md hover:-translate-y-1 transition-all duration-300 cursor-none" data-skill-title="Teamwork & Collaboration" data-skill-desc="Proven resilience in high-volume, peak conditions. Experienced in direct database logistics, member recruitment, and aligning operations with multi-stakeholder guidelines." data-skill-progress="88" data-skill-tag="Operations & Office">
                            <div class="w-10 h-10 rounded-xl bg-gray-100 flex items-center justify-center mb-4">
                                <i class="fa-solid fa-users text-pink-400 text-sm"></i>
                            </div>
                            <h3 class="text-xs uppercase tracking-wider font-semibold text-brand-dark mb-1">Teamwork & Office</h3>
                            <span class="text-[9px] uppercase tracking-wider text-brand-muted">Excel / Organization</span>
                        </div>

                    </div>
                    
                    <div class="flex justify-between items-center px-4 mt-2">
                        <span class="text-[9px] text-gray-400 uppercase tracking-widest flex items-center gap-1">
                            <i class="fa-solid fa-caret-left animate-pulse"></i> Drag to scroll
                        </span>
                        <span class="text-[9px] text-pink-400 uppercase tracking-widest">
                            Click card to inspect details
                        </span>
                    </div>
                </div>

                <div class="w-full max-w-2xl mx-auto pt-16">
                    <div class="relative mx-auto w-[90%] aspect-[16/10] bg-zinc-900 rounded-t-3xl border-[10px] border-zinc-900 shadow-2xl overflow-hidden flex flex-col justify-between">
                        <div class="absolute top-[3px] left-1/2 -translate-x-1/2 w-1.5 h-1.5 rounded-full bg-zinc-800"></div>
                        
                        <div id="mac-screen" class="w-full h-full bg-[#151517] p-6 text-white flex flex-col justify-between transition-all duration-500 overflow-hidden relative">
                            <div class="absolute inset-0 bg-[linear-gradient(to_right,#80808008_1px,transparent_1px),linear-gradient(to_bottom,#80808008_1px,transparent_1px)] bg-[size:15px_24px] pointer-events-none"></div>
                            
                            <div class="flex justify-between items-center border-b border-zinc-800/80 pb-3 z-10">
                                <div class="flex items-center gap-1.5">
                                    <span class="w-2.5 h-2.5 rounded-full bg-red-500/80"></span>
                                    <span class="w-2.5 h-2.5 rounded-full bg-yellow-500/80"></span>
                                    <span class="w-2.5 h-2.5 rounded-full bg-green-500/80"></span>
                                </div>
                                <span class="text-[9px] uppercase tracking-[0.2em] text-zinc-500 font-mono">competence_matrix_inspect.sh</span>
                                <span class="text-[9px] font-mono text-pink-400/80" id="mac-active-tag">PRODUCT DEMONSTRATION</span>
                            </div>

                            <div class="flex-grow flex flex-col justify-center items-start text-left py-4 z-10">
                                <h4 id="mac-skill-title" class="text-base md:text-lg font-light tracking-wide text-zinc-100 mb-2 uppercase transition-all duration-300">
                                    Product Education & Promotion
                                </h4>
                                <p id="mac-skill-desc" class="text-xs font-light text-zinc-400 leading-relaxed max-w-md h-16 overflow-y-auto pr-2 transition-all duration-300 no-scrollbar">
                                    Skilled at translating complex scientific, chemical, or formulation parameters into logical user benefits. Experienced performing technical presentations and live demonstrations to engage and convert clients.
                                </p>
                                
                                <div class="w-full max-w-sm mt-4">
                                    <div class="flex justify-between text-[9px] text-zinc-500 mb-1.5 font-mono">
                                        <span>RELEVANCE_COEFFICIENT</span>
                                        <span id="mac-skill-percentage" class="text-pink-400">95%</span>
                                    </div>
                                    <div class="w-full h-1 bg-zinc-800 rounded-full overflow-hidden">
                                        <div id="mac-skill-bar" class="h-full bg-gradient-to-r from-pink-500/80 to-pink-400 rounded-full transition-all duration-700 ease-out" style="width: 95%;"></div>
                                    </div>
                                </div>
                            </div>

                            <div class="flex justify-between items-center border-t border-zinc-800/80 pt-3 text-[9px] font-mono text-zinc-500 z-10">
                                <span>$ query --student "Allie Woon"</span>
                                <span>Status: Active Evaluation</span>
                            </div>
                        </div>
                    </div>

                    <div class="relative mx-auto w-full h-[14px] bg-[#d2d2d7] rounded-t-[1px] rounded-b-xl border-t border-white/60 shadow-[0_15px_30px_rgba(0,0,0,0.1)] flex justify-center">
                        <div class="w-16 h-1.5 bg-[#96969a] rounded-b-md absolute top-0"></div>
                    </div>
                    <div class="w-[96%] mx-auto h-[4px] bg-black/10 rounded-full blur-[2px] mt-1"></div>
                </div>

            </div>

        </div>
    </section>

    <section id="experience" class="min-h-screen py-32 px-6 md:px-12 lg:px-24 bg-white relative flex flex-col justify-center">
        <div class="max-w-5xl mx-auto w-full">
            
            <div class="mb-20">
                <span class="text-xs uppercase tracking-[0.4em] text-pink-400 font-light block mb-2">03 / EXPERIENCE</span>
                <h2 class="text-2xl font-light tracking-wide text-brand-dark uppercase">Professional History</h2>
                <div class="w-12 h-[1px] bg-pink-200 mt-4"></div>
            </div>

            <div class="space-y-12">
                
                <!-- HEYTEA Australia -->
                <div class="grid grid-cols-1 md:grid-cols-12 gap-6 md:gap-8 pb-10 border-b border-gray-100 group">
                    <div class="md:col-span-3">
                        <span class="text-xs uppercase tracking-[0.2em] text-brand-muted block mt-1">2026</span>
                        <span class="text-[10px] uppercase tracking-[0.1em] text-pink-400 block mt-1">Melbourne, AU</span>
                    </div>
                    <div class="md:col-span-9 space-y-3">
                        <div class="flex items-baseline justify-between">
                            <h3 class="text-base font-normal text-brand-dark">F&B Operations Staff @ HEYTEA</h3>
                        </div>
                        <p class="text-xs text-brand-muted leading-relaxed">
                            Thrived in a high-volume, extremely fast-paced hospitality environment. Coordinated order execution and cash/register reconciliations under peak pressure. Cultivated high performance, rigorous detail accuracy, and outstanding teamwork.
                        </p>
                        <p class="text-[11px] text-pink-400 italic">
                            Core Skill Transferability: Multi-tasking, structured team communication, and procedural compliance (highly valued in Clinical Trial Coordination and Trial assistant workflows).
                        </p>
                    </div>
                </div>

                <!-- Weekend Market Sales Assistant -->
                <div class="grid grid-cols-1 md:grid-cols-12 gap-6 md:gap-8 pb-10 border-b border-gray-100 group">
                    <div class="md:col-span-3">
                        <span class="text-xs uppercase tracking-[0.2em] text-brand-muted block mt-1">2026</span>
                        <span class="text-[10px] uppercase tracking-[0.1em] text-pink-400 block mt-1">Victoria, AU</span>
                    </div>
                    <div class="md:col-span-9 space-y-3">
                        <div class="flex items-baseline justify-between">
                            <h3 class="text-base font-normal text-brand-dark">Weekend Market Sales Assistant @ St Kilda & St Anglis Market</h3>
                        </div>
                        <p class="text-xs text-brand-muted leading-relaxed">
                            Engaged with a broad demographic of customers directly in bustling market settings. Controlled inventory logs, managed cash and digital POS systems securely, and built customer trust in face-to-face environments.
                        </p>
                        <p class="text-[11px] text-pink-400 italic">
                            Core Skill Transferability: Exceptional confidence, objection handling, persuasive sales drive, and personal customer relations.
                        </p>
                    </div>
                </div>

                <!-- Product Promoter Vinda -->
                <div class="grid grid-cols-1 md:grid-cols-12 gap-6 md:gap-8 pb-10 border-b border-gray-100 group">
                    <div class="md:col-span-3">
                        <span class="text-xs uppercase tracking-[0.2em] text-brand-muted block mt-1">2025</span>
                        <span class="text-[10px] uppercase tracking-[0.1em] text-pink-400 block mt-1">Kuala Lumpur, MY</span>
                    </div>
                    <div class="md:col-span-9 space-y-3">
                        <div class="flex items-baseline justify-between">
                            <h3 class="text-base font-normal text-brand-dark">Product Promoter @ Vinda</h3>
                        </div>
                        <p class="text-xs text-brand-muted leading-relaxed">
                            Represented leading hygiene and product brands through active demonstrations. Addressed target customer inquiries regarding scientific product formulations and features, achieving in-store conversion objectives.
                        </p>
                        <p class="text-[11px] text-pink-400 italic">
                            Core Skill Transferability: Scientific product translation, territory demonstration campaigns, and consultative product advocacy (ideal for Medical Device Specialists).
                        </p>
                    </div>
                </div>

                <!-- Sales Associate Nitori -->
                <div class="grid grid-cols-1 md:grid-cols-12 gap-6 md:gap-8 pb-10 border-b border-gray-100 group">
                    <div class="md:col-span-3">
                        <span class="text-xs uppercase tracking-[0.2em] text-brand-muted block mt-1">2024</span>
                        <span class="text-[10px] uppercase tracking-[0.1em] text-pink-400 block mt-1">Selangor, MY</span>
                    </div>
                    <div class="md:col-span-9 space-y-3">
                        <div class="flex items-baseline justify-between">
                            <h3 class="text-base font-normal text-brand-dark">Sales Associate @ Nitori</h3>
                        </div>
                        <p class="text-xs text-brand-muted leading-relaxed">
                            Delivered consultancies on domestic products in a high-traffic international showroom. Managed stock levels, verified promotional detail accuracy, and handled customer escalations.
                        </p>
                    </div>
                </div>

            </div>

            <!-- Leadership, Activities & Healthcare Volunteering (Strategic Addition) -->
            <div class="mt-24 pt-16 border-t border-gray-100">
                <div class="mb-12">
                    <span class="text-xs uppercase tracking-[0.4em] text-pink-400 font-light block mb-2">CLUBS & ACTIVITIES</span>
                    <h3 class="text-xl font-light tracking-wide text-brand-dark uppercase">Leadership & Activities</h3>
                    <div class="w-12 h-[1px] bg-pink-200 mt-3"></div>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                    <!-- Monash Investment Group -->
                    <div class="p-5 border border-gray-100 rounded-2xl hover:bg-neutral-50/40 transition-colors">
                        <div class="flex justify-between items-center mb-2">
                            <span class="text-[9px] uppercase font-mono tracking-wider text-pink-500">Business Drive</span>
                            <span class="text-[10px] text-gray-400">2025</span>
                        </div>
                        <h4 class="text-xs font-medium text-brand-dark">Monash Investment Group</h4>
                        <p class="text-[11px] text-brand-muted uppercase tracking-wider mt-0.5">HR Officer</p>
                        <p class="text-xs text-brand-muted mt-3 font-light leading-relaxed">
                            Coordinated candidate screening and recruitment logs. Highlights commercial business mindset and interest in professional management.
                        </p>
                    </div>

                    <!-- TEDx MCKL -->
                    <div class="p-5 border border-gray-100 rounded-2xl hover:bg-neutral-50/40 transition-colors">
                        <div class="flex justify-between items-center mb-2">
                            <span class="text-[9px] uppercase font-mono tracking-wider text-pink-500">Publicity & Media</span>
                            <span class="text-[10px] text-gray-400">2023</span>
                        </div>
                        <h4 class="text-xs font-medium text-brand-dark">MCKL TEDx Club</h4>
                        <p class="text-[11px] text-brand-muted uppercase tracking-wider mt-0.5">Publicity Team</p>
                        <p class="text-xs text-brand-muted mt-3 font-light leading-relaxed">
                            Created and scheduled promotional media. Refined strategic digital copywriting and multi-channel brand outreach.
                        </p>
                    </div>

                    <!-- Psychological First Aid Volunteer -->
                    <div class="p-5 border border-gray-100 rounded-2xl hover:bg-neutral-50/40 transition-colors">
                        <div class="flex justify-between items-center mb-2">
                            <span class="text-[9px] uppercase font-mono tracking-wider text-pink-500">Healthcare Volunteer</span>
                            <span class="text-[10px] text-gray-400">2022</span>
                        </div>
                        <h4 class="text-xs font-medium text-brand-dark">Psychological First Aid Workshop</h4>
                        <p class="text-[11px] text-brand-muted uppercase tracking-wider mt-0.5">Event Logistics</p>
                        <p class="text-xs text-brand-muted mt-3 font-light leading-relaxed">
                            Managed event setups, supported workshop delivery, and assisted vulnerable participants in health awareness initiatives.
                        </p>
                    </div>
                </div>
            </div>

        </div>
    </section>

    <section id="blueprints" class="min-h-screen py-32 px-6 md:px-12 lg:px-24 bg-gray-50/50 relative flex flex-col justify-center">
        <div class="max-w-7xl mx-auto w-full">
            
            <div class="mb-20 text-center md:text-left flex flex-col md:flex-row md:items-end md:justify-between gap-4">
                <div>
                    <span class="text-xs uppercase tracking-[0.4em] text-pink-400 font-light block mb-2">04 / BLUEPRINTS</span>
                    <h2 class="text-2xl font-light tracking-wide text-brand-dark uppercase">Graduate Career Targets</h2>
                </div>
                <div class="text-xs text-brand-muted tracking-[0.15em] uppercase font-light">
                    Focused Industrial Alignment
                </div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                
                <!-- Clinical Research -->
                <div class="bg-white border border-gray-200/50 rounded-3xl p-8 shadow-sm hover:shadow-md transition-all duration-300 flex flex-col justify-between">
                    <div>
                        <div class="flex justify-between items-center mb-6">
                            <div class="px-3 py-1 bg-pink-50 border border-pink-100 rounded-full text-[10px] font-semibold text-pink-500 uppercase tracking-widest">
                                Clinical Research / Operations
                            </div>
                            <span class="text-xs text-yellow-400 font-bold"><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i></span>
                        </div>
                        <h3 class="text-base font-normal text-brand-dark mb-4">Clinical Trial Coordination & Administration</h3>
                        <p class="text-xs text-brand-muted leading-relaxed mb-6">
                            Utilizes Monash Pharmaceutical Science training and professional organization to monitor trials, coordinate schedules, and manage secure documentation databases under ICH-GCP.
                        </p>
                        <div class="space-y-2 border-t border-gray-100 pt-4">
                            <div class="flex justify-between items-center text-[10px] text-brand-dark uppercase">
                                <span>Immediate:</span>
                                <span class="font-normal text-pink-500">Clinical Trial Assistant (CTA) / Coordinator (CRC)</span>
                            </div>
                            <div class="flex justify-between items-center text-[10px] text-gray-400 uppercase">
                                <span>Future:</span>
                                <span>Clinical Research Associate (CRA) / Clinical Project Manager</span>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Medical Devices -->
                <div class="bg-white border border-gray-200/50 rounded-3xl p-8 shadow-sm hover:shadow-md transition-all duration-300 flex flex-col justify-between">
                    <div>
                        <div class="flex justify-between items-center mb-6">
                            <div class="px-3 py-1 bg-pink-50 border border-pink-100 rounded-full text-[10px] font-semibold text-pink-500 uppercase tracking-widest">
                                Medical Devices
                            </div>
                            <span class="text-xs text-yellow-400 font-bold"><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i></span>
                        </div>
                        <h3 class="text-base font-normal text-brand-dark mb-4">Clinical Specialist & Territory Support</h3>
                        <p class="text-xs text-brand-muted leading-relaxed mb-6">
                            Combines clinical/biological understanding with persuasive promoter and direct sales experience to demonstrate tech products and support regional client accounts.
                        </p>
                        <div class="space-y-2 border-t border-gray-100 pt-4">
                            <div class="flex justify-between items-center text-[10px] text-brand-dark uppercase">
                                <span>Immediate:</span>
                                <span class="font-normal text-pink-500">Associate Clinical Specialist / Territory Associate</span>
                            </div>
                            <div class="flex justify-between items-center text-[10px] text-gray-400 uppercase">
                                <span>Future:</span>
                                <span>Clinical Specialist / Territory Manager / Product Specialist</span>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Pharma Commercial -->
                <div class="bg-white border border-gray-200/50 rounded-3xl p-8 shadow-sm hover:shadow-md transition-all duration-300 flex flex-col justify-between">
                    <div>
                        <div class="flex justify-between items-center mb-6">
                            <div class="px-3 py-1 bg-neutral-50 border border-neutral-200 rounded-full text-[10px] font-semibold text-zinc-500 uppercase tracking-widest">
                                Pharma Commercial
                            </div>
                            <span class="text-xs text-yellow-400 font-bold"><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i></span>
                        </div>
                        <h3 class="text-base font-normal text-brand-dark mb-4">Commercial Operations & Graduate BD</h3>
                        <p class="text-xs text-brand-muted leading-relaxed mb-6">
                            Expands sales opportunities utilizing bilingual capabilities, active regional campaign execution, and marketing analytics (MCKL TEDx publicity experience).
                        </p>
                        <div class="space-y-2 border-t border-gray-100 pt-4">
                            <div class="flex justify-between items-center text-[10px] text-brand-dark uppercase">
                                <span>Immediate:</span>
                                <span class="font-normal text-pink-500">Commercial Graduate / Sales Representative / BD Associate</span>
                            </div>
                            <div class="flex justify-between items-center text-[10px] text-gray-400 uppercase">
                                <span>Future:</span>
                                <span>Product Manager / Business Development Manager</span>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Health Tech -->
                <div class="bg-white border border-gray-200/50 rounded-3xl p-8 shadow-sm hover:shadow-md transition-all duration-300 flex flex-col justify-between">
                    <div>
                        <div class="flex justify-between items-center mb-6">
                            <div class="px-3 py-1 bg-neutral-50 border border-neutral-200 rounded-full text-[10px] font-semibold text-zinc-500 uppercase tracking-widest">
                                Health Tech
                            </div>
                            <span class="text-xs text-yellow-400 font-bold"><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i></span>
                        </div>
                        <h3 class="text-base font-normal text-brand-dark mb-4">Operations & Customer Onboarding</h3>
                        <p class="text-xs text-brand-muted leading-relaxed mb-6">
                            Brings structured fast-paced operational multitasking from busy client shifts into software, system implementations, and onboarding workflows.
                        </p>
                        <div class="space-y-2 border-t border-gray-100 pt-4">
                            <div class="flex justify-between items-center text-[10px] text-brand-dark uppercase">
                                <span>Immediate:</span>
                                <span class="font-normal text-pink-500">Operations Associate / Customer Success</span>
                            </div>
                            <div class="flex justify-between items-center text-[10px] text-gray-400 uppercase">
                                <span>Future:</span>
                                <span>Operations Manager / Product Operations Lead</span>
                            </div>
                        </div>
                    </div>
                </div>

            </div>

        </div>
    </section>

    <section id="ai-copilot" class="min-h-screen py-32 px-6 md:px-12 lg:px-24 bg-white relative flex flex-col justify-center">
        <div class="max-w-7xl mx-auto w-full space-y-16">
            
            <div class="text-center md:text-left">
                <span class="text-xs uppercase tracking-[0.4em] text-pink-400 font-light block mb-2">05 / AI CO-PILOT ARCHIVE</span>
                <h2 class="text-2xl font-light tracking-wide text-brand-dark uppercase">Recruiter AI Studio</h2>
                <div class="w-12 h-[1px] bg-pink-200 mt-4 mx-auto md:mx-0"></div>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-stretch">
                
                <!-- Chat Window -->
                <div class="lg:col-span-7 flex flex-col bg-gray-50/50 border border-gray-100 rounded-3xl p-6 md:p-8 justify-between relative overflow-hidden">
                    <div>
                        <div class="flex justify-between items-center pb-4 border-b border-gray-200/40 mb-6">
                            <div class="flex items-center gap-2">
                                <span class="relative flex h-2 w-2">
                                    <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-pink-400 opacity-75"></span>
                                    <span class="relative inline-flex rounded-full h-2 w-2 bg-pink-500"></span>
                                </span>
                                <h3 class="text-xs uppercase tracking-[0.25em] text-brand-dark font-medium">CHAT WITH ALLIE'S AVATAR</h3>
                            </div>
                            <span class="text-[9px] font-mono text-brand-muted uppercase bg-white px-2.5 py-1 rounded-full border border-gray-100">gemini-3-flash</span>
                        </div>

                        <div id="ai-chat-thread" class="space-y-4 max-h-[340px] overflow-y-auto pr-2 no-scrollbar min-h-[250px]">
                            <div class="flex items-start gap-3">
                                <div class="w-7 h-7 rounded-full bg-pink-100 flex items-center justify-center text-[10px] text-pink-400 font-medium">AI</div>
                                <div class="bg-white border border-gray-100/80 rounded-2xl rounded-tl-none p-3 max-w-[85%]">
                                    <p class="text-xs text-brand-dark leading-relaxed font-light">
                                        Hello! I am Allie's AI assistant. Ask me how her Monash Pharmaceutical Science training, coursework (Pharmacology, Formulation), and high-confidence Australia commercial background fit your openings in Clinical Operations, Medical Devices, Commercial Pharma, or Health Tech!
                                    </p>
                                    <div class="flex flex-wrap gap-2 mt-3">
                                        <button class="prompt-chip px-3 py-1 bg-gray-50 border border-gray-100 rounded-full text-[10px] text-brand-muted hover:border-pink-300 hover:text-pink-500 transition-all duration-300 cursor-none">How do your skills match a Clinical Research Assistant role?</button>
                                        <button class="prompt-chip px-3 py-1 bg-gray-50 border border-gray-100 rounded-full text-[10px] text-brand-muted hover:border-pink-300 hover:text-pink-500 transition-all duration-300 cursor-none">Why are you suitable for a Medical Device Specialist role?</button>
                                        <button class="prompt-chip px-3 py-1 bg-gray-50 border border-gray-100 rounded-full text-[10px] text-brand-muted hover:border-pink-300 hover:text-pink-500 transition-all duration-300 cursor-none">Detail your academic coursework and background</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="mt-6 pt-4 border-t border-gray-200/40">
                        <form id="ai-chat-form" class="flex items-center gap-2">
                            <input id="ai-chat-input" type="text" autocomplete="off" placeholder="Ask about Allie's coursework, trial assistant fit, device promotion..." class="flex-grow bg-white border border-gray-200 rounded-full py-3 px-5 text-xs text-brand-dark focus:outline-none focus:border-pink-300 transition-colors placeholder-gray-400 cursor-none">
                            <button type="submit" class="w-10 h-10 bg-brand-dark hover:bg-zinc-800 rounded-full flex items-center justify-center text-white transition-all duration-300 group cursor-none">
                                <i class="fa-solid fa-arrow-up text-xs group-hover:translate-y-[-2.5px] transition-transform"></i>
                            </button>
                        </form>
                    </div>

                    <!-- TTS Floating Synthesizer visualizer block -->
                    <div id="voice-visualizer" class="absolute bottom-16 right-6 bg-white/90 backdrop-blur border border-pink-100 px-4 py-2 rounded-full flex items-center gap-2.5 shadow-sm opacity-0 scale-90 pointer-events-none transition-all duration-300">
                        <span class="text-[9px] uppercase tracking-widest text-pink-500 font-mono">Synthesizing Voice...</span>
                        <div class="flex items-end gap-0.5 h-3">
                            <span class="w-0.5 bg-pink-400 rounded-full animate-[bounce_0.8s_infinite]"></span>
                            <span class="w-0.5 bg-pink-400 rounded-full animate-[bounce_0.5s_infinite_0.1s]"></span>
                            <span class="w-0.5 bg-pink-400 rounded-full animate-[bounce_0.7s_infinite_0.2s]"></span>
                            <span class="w-0.5 bg-pink-400 rounded-full animate-[bounce_0.4s_infinite_0.3s]"></span>
                        </div>
                        <button id="stop-voice-btn" class="text-[10px] text-gray-400 hover:text-pink-500 ml-1 cursor-none"><i class="fa-solid fa-circle-stop"></i></button>
                    </div>
                </div>

                <!-- Matcher Evaluation Desk -->
                <div class="lg:col-span-5 bg-[#141416] text-white rounded-3xl p-6 md:p-8 flex flex-col justify-between relative overflow-hidden">
                    <div class="absolute inset-0 bg-[linear-gradient(to_right,#80808005_1px,transparent_1px),linear-gradient(to_bottom,#80808005_1px,transparent_1px)] bg-[size:16px_16px] pointer-events-none"></div>

                    <div class="z-10 space-y-6">
                        <div class="flex justify-between items-center pb-4 border-b border-zinc-800/80">
                            <div class="flex items-center gap-2">
                                <i class="fa-solid fa-briefcase text-pink-400 text-xs"></i>
                                <h3 class="text-xs uppercase tracking-[0.25em] text-zinc-100 font-medium font-mono">JD COMPATIBILITY MATRIX</h3>
                            </div>
                            <span class="text-[9px] font-mono text-zinc-500">MATRIX EVAL</span>
                        </div>

                        <p class="text-xs text-zinc-400 leading-relaxed font-light">
                            Paste any graduate or professional Job Description (Clinical Research Assistant, Medical Device Sales, Commercial Associate, etc.) to immediately test compatibility.
                        </p>

                        <div class="space-y-3">
                            <textarea id="jd-textarea" placeholder="Paste a job description here (e.g. 'Looking for a Clinical Research Assistant with strong science background, communication, and meticulous documentation skills...')" class="w-full h-28 bg-zinc-900 border border-zinc-800 rounded-2xl p-4 text-xs text-zinc-100 focus:outline-none focus:border-pink-500 transition-colors placeholder-zinc-600 resize-none font-light leading-relaxed cursor-none"></textarea>
                            <button id="analyze-jd-btn" type="button" class="w-full py-3 bg-white hover:bg-zinc-200 text-brand-dark rounded-full text-xs uppercase tracking-[0.2em] font-normal transition-all duration-300 flex items-center justify-center gap-2 cursor-none">
                                <i class="fa-solid fa-calculator text-pink-500"></i> Run Suitability Analysis
                            </button>
                        </div>

                        <!-- Results Dashboard -->
                        <div id="analysis-dashboard" class="hidden border border-zinc-800 rounded-2xl p-4 space-y-4 bg-zinc-900/40 backdrop-blur-md transition-all duration-500">
                            <div class="flex items-center justify-between">
                                <span class="text-[10px] tracking-widest text-zinc-400 uppercase font-mono">MATCHING_ACCURACY</span>
                                <span id="match-score" class="text-base font-mono text-pink-400 font-semibold">95%</span>
                            </div>
                            <div class="w-full h-1 bg-zinc-800 rounded-full overflow-hidden">
                                <div id="match-score-bar" class="h-full bg-pink-500 rounded-full transition-all duration-1000" style="width: 0%;"></div>
                            </div>
                            <div class="space-y-2">
                                <span class="text-[10px] tracking-widest text-zinc-400 uppercase block font-mono">TAILORED_PITCH</span>
                                <p id="match-summary" class="text-[11px] text-zinc-300 font-light leading-relaxed max-h-[120px] overflow-y-auto pr-1 no-scrollbar text-justify"></p>
                            </div>
                        </div>
                    </div>

                    <div class="border-t border-zinc-800/80 pt-4 mt-6 text-[9px] font-mono text-zinc-500 flex justify-between items-center z-10">
                        <span>$ python compatibility_eval.py</span>
                        <span>STATUS: SYSTEM_READY</span>
                    </div>
                </div>

            </div>

        </div>
    </section>

    <section id="contact-me" class="min-h-screen py-32 px-6 md:px-12 lg:px-24 bg-white relative flex flex-col justify-center">
        <div class="max-w-4xl mx-auto w-full text-center space-y-12">
            
            <div class="space-y-4">
                <span class="text-xs uppercase tracking-[0.4em] text-pink-400 font-light block">05 / GET IN TOUCH</span>
                <h2 class="text-3xl md:text-5xl font-light tracking-wide text-brand-dark uppercase">Let's Connect</h2>
                <p class="text-xs md:text-sm text-brand-muted tracking-wider max-w-lg mx-auto leading-relaxed">
                    If you have a role matching Allie's pharmaceutical science background, direct communication, and commercial drive, let's explore professional synergies.
                </p>
            </div>

            <div class="flex flex-col sm:flex-row justify-center items-center gap-4 pt-6">
                <a href="mailto:allywoonzhiyu@gmail.com" class="w-full sm:w-auto px-8 py-4 border border-gray-200 rounded-full text-xs uppercase tracking-[0.25em] font-normal text-brand-dark hover:border-pink-300 hover:bg-pink-50/10 transition-all duration-300 flex items-center justify-center gap-2 cursor-none">
                    <i class="fa-regular fa-envelope text-pink-400"></i> allywoonzhiyu@gmail.com
                </a>
                <a href="tel:0412260659" class="w-full sm:w-auto px-8 py-4 bg-brand-dark hover:bg-zinc-800 rounded-full text-xs uppercase tracking-[0.25em] font-normal text-white transition-all duration-300 flex items-center justify-center gap-2 cursor-none">
                    <i class="fa-solid fa-phone text-pink-300"></i> +61 412 260 659
                </a>
            </div>

            <div class="pt-24 border-t border-gray-100 flex flex-col md:flex-row justify-between items-center text-[10px] text-brand-muted tracking-[0.2em] uppercase gap-4">
                <span>© 2026 Allie Woon. All rights reserved.</span>
                <span>MONASH PHARMACEUTICAL SCIENCE</span>
                <span class="text-[9px] text-gray-400">MADE WITH SOURce HAN SANS</span>
            </div>

        </div>
    </section>

    <script>
        document.addEventListener('DOMContentLoaded', () => {

            // ==========================================
            // 1. Premium Custom Cursor Movements & LERP
            // ==========================================
            const cursorDot = document.getElementById('cursor-dot');
            const cursorOutline = document.getElementById('cursor-outline');

            let mouseX = window.innerWidth / 2;
            let mouseY = window.innerHeight / 2;
            let outlineX = mouseX;
            let outlineY = mouseY;

            window.addEventListener('mousemove', (e) => {
                mouseX = e.clientX;
                mouseY = e.clientY;

                cursorDot.style.left = `${mouseX}px`;
                cursorDot.style.top = `${mouseY}px`;
            });

            const animateOutlineCursor = () => {
                const speed = 0.15;
                outlineX += (mouseX - outlineX) * speed;
                outlineY += (mouseY - outlineY) * speed;

                cursorOutline.style.left = `${outlineX}px`;
                cursorOutline.style.top = `${outlineY}px`;

                requestAnimationFrame(animateOutlineCursor);
            };
            animateOutlineCursor();

            const targetInteractiveTags = document.querySelectorAll('a, button, .skill-card, #directory-trigger h1, .prompt-chip, input, textarea');
            targetInteractiveTags.forEach(elem => {
                elem.addEventListener('mouseenter', () => {
                    cursorOutline.classList.add('w-14', 'h-14', 'border-pink-500/70', 'bg-pink-300/20');
                    cursorDot.classList.add('scale-150', 'bg-pink-600');
                });
                elem.addEventListener('mouseleave', () => {
                    cursorOutline.classList.remove('w-14', 'h-14', 'border-pink-500/70', 'bg-pink-300/20');
                    cursorDot.classList.remove('scale-150', 'bg-pink-600');
                });
            });


            // ==========================================
            // 2. Index Dropdown Hover Staggered Effect
            // ==========================================
            const directoryTrigger = document.getElementById('directory-trigger');
            const dropdownContainer = document.getElementById('directory-dropdown');
            const dropdownItems = document.querySelectorAll('.directory-item');

            let closeTimer;

            directoryTrigger.addEventListener('mouseenter', () => {
                clearTimeout(closeTimer);
                dropdownContainer.classList.remove('opacity-0', 'pointer-events-none', 'scale-95');
                dropdownContainer.classList.add('opacity-100', 'pointer-events-auto', 'scale-100');

                dropdownItems.forEach((item) => {
                    item.classList.remove('opacity-0', '-translate-y-2');
                    item.classList.add('opacity-100', 'translate-y-0');
                });
            });

            directoryTrigger.addEventListener('mouseleave', () => {
                closeTimer = setTimeout(() => {
                    closeDropdownMenu();
                }, 300);
            });

            dropdownContainer.addEventListener('mouseenter', () => {
                clearTimeout(closeTimer);
            });

            dropdownContainer.addEventListener('mouseleave', () => {
                closeTimer = setTimeout(() => {
                    closeDropdownMenu();
                }, 200);
            });

            function closeDropdownMenu() {
                dropdownContainer.classList.remove('opacity-100', 'pointer-events-auto', 'scale-100');
                dropdownContainer.classList.add('opacity-0', 'pointer-events-none', 'scale-95');

                dropdownItems.forEach((item) => {
                    item.classList.remove('opacity-100', 'translate-y-0');
                    item.classList.add('opacity-0', '-translate-y-2');
                });
            }

            dropdownItems.forEach(item => {
                item.addEventListener('click', () => {
                    closeDropdownMenu();
                });
            });


            // ==========================================
            // 3. MacBook Skill Switcher Event Handler
            // ==========================================
            const skillCards = document.querySelectorAll('.skill-card');
            const macTitle = document.getElementById('mac-skill-title');
            const macDesc = document.getElementById('mac-skill-desc');
            const macTag = document.getElementById('mac-active-tag');
            const macPercentage = document.getElementById('mac-skill-percentage');
            const macBar = document.getElementById('mac-skill-bar');
            const macScreen = document.getElementById('mac-screen');

            skillCards[0].classList.add('border-pink-400', 'bg-white/90');

            skillCards.forEach(card => {
                card.addEventListener('click', () => {
                    skillCards.forEach(c => c.classList.remove('border-pink-400', 'bg-white/90'));
                    card.classList.add('border-pink-400', 'bg-white/90');

                    const title = card.getAttribute('data-skill-title');
                    const desc = card.getAttribute('data-skill-desc');
                    const progress = card.getAttribute('data-skill-progress');
                    const tag = card.getAttribute('data-skill-tag');

                    macScreen.classList.add('opacity-40');
                    
                    setTimeout(() => {
                        macTitle.textContent = title;
                        macDesc.textContent = desc;
                        macTag.textContent = tag.toUpperCase();
                        macPercentage.textContent = `${progress}%`;
                        macBar.style.width = `${progress}%`;
                        macScreen.classList.remove('opacity-40');
                    }, 200);
                });
            });

            const slider = document.getElementById('skills-cards-container');
            let isDown = false;
            let startX;
            let scrollLeft;

            slider.addEventListener('mousedown', (e) => {
                isDown = true;
                startX = e.pageX - slider.offsetLeft;
                scrollLeft = slider.scrollLeft;
            });
            slider.addEventListener('mouseleave', () => {
                isDown = false;
            });
            slider.addEventListener('mouseup', () => {
                isDown = false;
            });
            slider.addEventListener('mousemove', (e) => {
                if(!isDown) return;
                e.preventDefault();
                const x = e.pageX - slider.offsetLeft;
                const walk = (x - startX) * 1.5;
                slider.scrollLeft = scrollLeft - walk;
            });


            // ==========================================
            // 4. Gemini API Chat & Voice Synthesis Integration
            // ==========================================
            const apiKey = ""; // Canvas runtime keys fallback
            const modelName = "gemini-3-flash-preview";
            const ttsModelName = "gemini-2.5-flash-preview-tts";

            // Recruiter-optimised contextual parameters
            const resumeFacts = `
                Candidate Name: Allie Woon (Woon Zhi Yu)
                Education: Monash University Malaysia, Bachelor of Pharmaceutical Science (Expected 2027)
                Relevant Coursework: Pharmacology, Drug Discovery, Medicinal Chemistry, Human Physiology, Pharmaceutical Formulation.
                Professional Strategy Core Narrative: "Pharmaceutical Science student with strong communication and commercial skills interested in healthcare/pharma."
                
                Immediate Career Path Objectives:
                - Clinical Research / Operations: Clinical Trial Assistant (CTA), Clinical Research Coordinator (CRC).
                - Medical Devices: Associate Clinical Specialist, Sales Support, Territory Associate.
                - Pharma Commercial / Health Tech: Commercial Graduate, Operations Associate, Customer Success.
                
                Key Transferable Assets:
                1. Scientific Acumen: Solid monash pharmacology/formulation background (reminding recruiters of scientific rigor).
                2. Communication: Fluent in English and Mandarin, conversational Cantonese. Elite consultative relationship building.
                3. Commercial Drive & Multitasking: Experience in Australia (HEYTEA Australia, Weekend Market Sales) and Malaysia (Vinda promoter, Nitori sales associate).
                4. Business Coordination: HR officer for Monash University Investment Group (member records/recruitment logs), MCKL TEDx Club publicity team, Psychological First Aid workshop helper.
                
                Target Exclusions (DO NOT mention on query - keeps resume clean):
                - No casual hourly details, weekends-only tables, or visa details are listed directly. Address visa status (Student Visa) professionally when asked directly.
                - No minor/unrelated activities like badminton treasurer or office retail associate (removed to maintain high-impact professional focus).
            `;

            let activeAudioSession = null;

            const chatForm = document.getElementById('ai-chat-form');
            const chatInput = document.getElementById('ai-chat-input');
            const chatThread = document.getElementById('ai-chat-thread');
            const voiceVisualizer = document.getElementById('voice-visualizer');
            const stopVoiceBtn = document.getElementById('stop-voice-btn');

            const promptChips = document.querySelectorAll('.prompt-chip');
            promptChips.forEach(chip => {
                chip.addEventListener('click', () => {
                    chatInput.value = chip.textContent;
                    submitChatMessage();
                });
            });

            chatForm.addEventListener('submit', (e) => {
                e.preventDefault();
                submitChatMessage();
            });

            async function submitChatMessage() {
                const userText = chatInput.value.trim();
                if (!userText) return;

                appendBubble("user", userText);
                chatInput.value = "";

                const loadingIndicator = appendBubble("ai", `<span class="animate-pulse">Consulting clinical data...</span>`, true);

                try {
                    const systemInstructions = `You are the digital twin AI assistant of Allie Woon.
                    Provide professional, highly polished, and concise responses (maximum 3 sentences) fitting a premier scientific-commercial candidate.
                    Pitch Allie explicitly for roles in Clinical Research (CTA/CRC), Medical Devices (Clinical Specialist), Pharma Commercial, or Health Tech.
                    Frame her scientific training (Pharmacology, Formulation) and her communication drive (HEYTEA, Market Sales) as an elite combination.`;

                    const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/${modelName}:generateContent?key=${apiKey}`;
                    
                    const response = await fetch(apiUrl, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify({
                            contents: [{ parts: [{ text: `User query: ${userText}\nResume Context:\n${resumeFacts}` }] }],
                            systemInstruction: { parts: [{ text: systemInstructions }] }
                        })
                    });

                    if (!response.ok) throw new Error("Connection failed");
                    const data = await response.json();
                    const rawResult = data.candidates?.[0]?.content?.parts?.[0]?.text || "Allie is prepared for high-impact Clinical Trial Assistant or Medical Device Associate positions. Contact her at allywoonzhiyu@gmail.com.";

                    loadingIndicator.id = "msg-" + Date.now();
                    loadingIndicator.innerHTML = `
                        <p class="text-xs text-brand-dark leading-relaxed font-light">${rawResult.replace(/\n/g, '<br>')}</p>
                        <div class="mt-2 flex gap-2">
                            <button onclick="speakResponse(this, '${rawResult.replace(/'/g, "\\'")}')" class="text-[9px] uppercase tracking-widest text-pink-500 font-medium hover:text-pink-600 transition-colors flex items-center gap-1.5 bg-pink-50/50 hover:bg-pink-50 border border-pink-100 rounded-full px-2.5 py-1 cursor-none">
                                <i class="fa-solid fa-volume-high"></i> Listen to Response
                            </button>
                        </div>
                    `;
                } catch (e) {
                    console.error("API Assistant failure:", e);
                    loadingIndicator.innerHTML = `<span class="text-xs text-red-400">Connection error. Please reach out to Allie directly via allywoonzhiyu@gmail.com!</span>`;
                }

                chatThread.scrollTop = chatThread.scrollHeight;
            }

            function appendBubble(role, text, isLoading = false) {
                const row = document.createElement('div');
                row.className = "flex items-start gap-3 " + (role === "user" ? "justify-end" : "");

                if (role === "user") {
                    row.innerHTML = `
                        <div class="bg-pink-100/40 border border-pink-100/60 rounded-2xl rounded-tr-none p-3 max-w-[85%]">
                            <p class="text-xs text-brand-dark leading-relaxed font-light">${text}</p>
                        </div>
                        <div class="w-7 h-7 rounded-full bg-brand-dark flex items-center justify-center text-[10px] text-white font-medium">U</div>
                    `;
                } else {
                    row.innerHTML = `
                        <div class="w-7 h-7 rounded-full bg-pink-100 flex items-center justify-center text-[10px] text-pink-400 font-medium">AI</div>
                        <div class="bg-white border border-gray-100/80 rounded-2xl rounded-tl-none p-3 max-w-[85%]">
                            ${isLoading ? text : `<p class="text-xs text-brand-dark leading-relaxed font-light">${text}</p>`}
                        </div>
                    `;
                }

                chatThread.appendChild(row);
                chatThread.scrollTop = chatThread.scrollHeight;
                return row.querySelector('.bg-white');
            }


            // ==========================================
            // 5. Job Description Compatibility Analyzer
            // ==========================================
            const analyzeBtn = document.getElementById('analyze-jd-btn');
            const jdTextarea = document.getElementById('jd-textarea');
            const analysisDashboard = document.getElementById('analysis-dashboard');
            const matchScoreSpan = document.getElementById('match-score');
            const matchScoreProgress = document.getElementById('match-score-bar');
            const matchSummaryText = document.getElementById('match-summary');

            analyzeBtn.addEventListener('click', async () => {
                const jdContent = jdTextarea.value.trim();
                if (!jdContent) return;

                analyzeBtn.disabled = true;
                analyzeBtn.innerHTML = `<i class="fa-solid fa-spinner animate-spin"></i> Running Analysis...`;
                analysisDashboard.classList.add('hidden');

                try {
                    const evaluationInstructions = `You are a professional life-sciences recruiter.
                    Evaluate how Allie Woon fits the job description. Allie's core profile is: "Pharmaceutical Science student with strong communication and commercial skills interested in healthcare/pharma."
                    Use her resume details:
                    ${resumeFacts}
                    
                    Respond ONLY with a valid JSON object. Do not wrap in markdown quotes.
                    The JSON must contain:
                    1. "score": an integer representing her fitness percentage (0 to 100), based on her Pharmacology/formulation coursework and high-confidence sales/promotion history.
                    2. "pitch": a highly tailored, persuasive 3-sentence summary highlighting why her bilingual fluency, scientific coursework, and commercial confidence (HEYTEA, Market Sales, Vinda promoter) fit the core criteria of this job description.`;

                    const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/${modelName}:generateContent?key=${apiKey}`;
                    
                    const res = await fetch(apiUrl, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify({
                            contents: [{ parts: [{ text: jdContent }] }],
                            generationConfig: { responseMimeType: "application/json" },
                            systemInstruction: { parts: [{ text: evaluationInstructions }] }
                        })
                    });

                    if (!res.ok) throw new Error("JSON generation failure.");
                    const responseData = await res.json();
                    const textContent = responseData.candidates?.[0]?.content?.parts?.[0]?.text;
                    const parsedData = JSON.parse(textContent);

                    analysisDashboard.classList.remove('hidden');
                    matchScoreSpan.textContent = `${parsedData.score}%`;
                    matchScoreProgress.style.width = `${parsedData.score}%`;
                    matchSummaryText.textContent = parsedData.pitch;

                } catch (err) {
                    console.error("Evaluation error:", err);
                    analysisDashboard.classList.remove('hidden');
                    matchScoreSpan.textContent = "N/A";
                    matchScoreProgress.style.width = "0%";
                    matchSummaryText.textContent = "Allie is highly ready with customer promotion, operations, and Monash scientific training. Contact her directly for custom scheduling.";
                } finally {
                    analyzeBtn.disabled = false;
                    analyzeBtn.innerHTML = `<i class="fa-solid fa-calculator text-pink-500"></i> Run Suitability Analysis`;
                }
            });


            // ==========================================
            // 6. Audio Synthesizer (TTS Voice Module)
            // ==========================================
            window.speakResponse = async (btn, speechContent) => {
                if (activeAudioSession) {
                    activeAudioSession.pause();
                    activeAudioSession = null;
                }

                voiceVisualizer.classList.remove('opacity-0', 'pointer-events-none', 'scale-90');
                voiceVisualizer.classList.add('opacity-100', 'pointer-events-auto', 'scale-100');

                btn.disabled = true;
                const innerHtmlBackup = btn.innerHTML;
                btn.innerHTML = `<i class="fa-solid fa-spinner animate-spin"></i> Translating...`;

                try {
                    const formattedText = speechContent.replace(/<[^>]*>/g, '');
                    const ttsUrl = `https://generativelanguage.googleapis.com/v1beta/models/${ttsModelName}:generateContent?key=${apiKey}`;

                    const response = await fetch(ttsUrl, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify({
                            contents: [{
                                parts: [{ text: `Speak in a warm, professional, highly polished female recruiter assistant tone: ${formattedText}` }]
                            }],
                            generationConfig: {
                                responseModalities: ["AUDIO"],
                                speechConfig: {
                                    voiceConfig: {
                                        prebuiltVoiceConfig: { voiceName: "Sulafat" } // Warm professional voice
                                    }
                                }
                            }
                        })
                    });

                    if (!response.ok) throw new Error("TTS Request Failed");
                    const result = await response.json();
                    
                    const part = result?.candidates?.[0]?.content?.parts?.[0];
                    const base64Data = part?.inlineData?.data;
                    const mimeType = part?.inlineData?.mimeType;

                    if (base64Data && mimeType && mimeType.startsWith("audio/")) {
                        const sRateMatch = mimeType.match(/rate=(\d+)/);
                        const sampleRate = sRateMatch ? parseInt(sRateMatch[1], 10) : 24000;
                        
                        const pcmData = b64ToArrayBuffer(base64Data);
                        const pcm16 = new Int16Array(pcmData);
                        const wavBlob = pcmToWavContainer(pcm16, sampleRate);
                        const audioUrl = URL.createObjectURL(wavBlob);

                        activeAudioSession = new Audio(audioUrl);
                        activeAudioSession.addEventListener('ended', () => {
                            hideVisualizerHUD();
                            btn.disabled = false;
                            btn.innerHTML = innerHtmlBackup;
                        });
                        activeAudioSession.play();
                    } else {
                        throw new Error("Invalid voice packaging");
                    }
                } catch (e) {
                    console.error("TTS processing error:", e);
                    hideVisualizerHUD();
                    btn.disabled = false;
                    btn.innerHTML = innerHtmlBackup;
                }
            };

            stopVoiceBtn.addEventListener('click', () => {
                if (activeAudioSession) {
                    activeAudioSession.pause();
                    activeAudioSession = null;
                }
                hideVisualizerHUD();
                const speakBtns = document.querySelectorAll('#ai-chat-thread button');
                speakBtns.forEach(btn => {
                    btn.disabled = false;
                    btn.innerHTML = `<i class="fa-solid fa-volume-high"></i> Listen to Response`;
                });
            });

            function hideVisualizerHUD() {
                voiceVisualizer.classList.add('opacity-0', 'pointer-events-none', 'scale-90');
                voiceVisualizer.classList.remove('opacity-100', 'pointer-events-auto', 'scale-100');
            }

            function b64ToArrayBuffer(base64) {
                const binStr = window.atob(base64);
                const bytes = new Uint8Array(binStr.length);
                for (let i = 0; i < binStr.length; i++) {
                    bytes[i] = binStr.charCodeAt(i);
                }
                return bytes.buffer;
            }

            function pcmToWavContainer(pcm16, sRate) {
                const buffer = new ArrayBuffer(44 + pcm16.length * 2);
                const view = new DataView(buffer);

                writeStringBytes(view, 0, 'RIFF');
                view.setUint32(4, 36 + pcm16.length * 2, true);
                writeStringBytes(view, 8, 'WAVE');
                writeStringBytes(view, 12, 'fmt ');
                view.setUint32(16, 16, true);
                view.setUint16(20, 1, true); // Raw signed PCM format
                view.setUint16(22, 1, true); // Mono channel
                view.setUint32(24, sRate, true);
                view.setUint32(28, sRate * 2, true);
                view.setUint16(32, 2, true);
                view.setUint16(34, 16, true);
                writeStringBytes(view, 36, 'data');
                view.setUint32(40, pcm16.length * 2, true);

                for (let i = 0; i < pcm16.length; i++) {
                    view.setInt16(44 + i * 2, pcm16[i], true);
                }

                return new Blob([view], { type: 'audio/wav' });
            }

            function writeStringBytes(view, offset, str) {
                for (let i = 0; i < str.length; i++) {
                    view.setUint8(offset + i, str.charCodeAt(i));
                }
            }

        });
    </script>
</body>
</html>
