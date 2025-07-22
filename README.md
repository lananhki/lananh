<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Professional CV</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: {
                            light: '#6366F1',
                            DEFAULT: '#4F46E5',
                            dark: '#4338CA',
                        },
                        secondary: {
                            light: '#F0FDFA',
                            DEFAULT: '#CCFBF1',
                            dark: '#14B8A6',
                        },
                        dark: {
                            light: '#334155',
                            DEFAULT: '#1E293B',
                            dark: '#0F172A',
                        }
                    },
                    fontFamily: {
                        sans: ['Poppins', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        
        html {
            scroll-behavior: smooth;
        }
        
        .animate-fade-in {
            animation: fadeIn 0.8s ease-in;
        }
        
        .animate-slide-up {
            animation: slideUp 0.8s ease-out;
        }
        
        .animate-slide-in {
            animation: slideIn 0.8s ease-out;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        @keyframes slideUp {
            from { transform: translateY(50px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }
        
        @keyframes slideIn {
            from { transform: translateX(-50px); opacity: 0; }
            to { transform: translateX(0); opacity: 1; }
        }
        
        .section-divider {
            height: 3px;
            background: linear-gradient(90deg, rgba(79,70,229,0) 0%, rgba(79,70,229,1) 50%, rgba(79,70,229,0) 100%);
            margin: 2rem 0;
        }
        
        .project-card {
            transition: all 0.3s ease;
        }
        
        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px -5px rgba(79, 70, 229, 0.3);
        }
        
        .skill-pill {
            transition: all 0.3s ease;
        }
        
        .skill-pill:hover {
            transform: scale(1.05);
            box-shadow: 0 4px 12px rgba(79, 70, 229, 0.2);
        }
        
        .nav-link {
            position: relative;
        }
        
        .nav-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -2px;
            left: 0;
            background-color: #4F46E5;
            transition: width 0.3s ease;
        }
        
        .nav-link:hover::after {
            width: 100%;
        }
        
        .active::after {
            width: 100%;
        }
        
        .glass-effect {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .gradient-text {
            background: linear-gradient(90deg, #4F46E5, #14B8A6);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        
        .gradient-bg {
            background: linear-gradient(135deg, #4F46E5, #14B8A6);
        }
        
        .shadow-custom {
            box-shadow: 0 10px 30px -5px rgba(79, 70, 229, 0.2);
        }
    </style>
</head>
<body class="bg-gray-50 text-dark font-sans">
    <!-- Header/Navigation -->
    <header class="fixed w-full bg-white bg-opacity-95 shadow-md z-50">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <h1 class="text-2xl font-bold">
                <span class="gradient-text">Professional</span> CV
            </h1>
            <nav class="hidden md:block">
                <ul class="flex space-x-6">
                    <li><a href="#intro" class="nav-link active font-medium hover:text-primary transition-colors">Home</a></li>
                    <li><a href="#about" class="nav-link font-medium hover:text-primary transition-colors">About</a></li>
                    <li><a href="#education" class="nav-link font-medium hover:text-primary transition-colors">Education</a></li>
                    <li><a href="#experience" class="nav-link font-medium hover:text-primary transition-colors">Experience</a></li>
                    <li><a href="#projects" class="nav-link font-medium hover:text-primary transition-colors">Projects</a></li>
                    <li><a href="#skills" class="nav-link font-medium hover:text-primary transition-colors">Skills</a></li>
                </ul>
            </nav>
            <button id="mobile-menu-button" class="md:hidden text-dark">
                <i class="fas fa-bars text-xl"></i>
            </button>
        </div>
        <!-- Mobile menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white shadow-lg absolute w-full">
            <ul class="flex flex-col py-2">
                <li><a href="#intro" class="block px-4 py-2 hover:bg-primary hover:text-white transition-colors">Home</a></li>
                <li><a href="#about" class="block px-4 py-2 hover:bg-primary hover:text-white transition-colors">About</a></li>
                <li><a href="#education" class="block px-4 py-2 hover:bg-primary hover:text-white transition-colors">Education</a></li>
                <li><a href="#experience" class="block px-4 py-2 hover:bg-primary hover:text-white transition-colors">Experience</a></li>
                <li><a href="#projects" class="block px-4 py-2 hover:bg-primary hover:text-white transition-colors">Projects</a></li>
                <li><a href="#skills" class="block px-4 py-2 hover:bg-primary hover:text-white transition-colors">Skills</a></li>
            </ul>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="intro" class="pt-24 pb-16 bg-gradient-to-br from-dark-dark via-primary-dark to-primary text-white">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 animate-fade-in">
                    <div class="bg-white rounded-full w-48 h-48 mx-auto md:mx-0 overflow-hidden border-4 border-white shadow-xl">
                        <svg class="w-full h-full text-gray-300" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M12 12c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm0 2c-2.67 0-8 1.34-8 4v2h16v-2c0-2.66-5.33-4-8-4z"></path>
                        </svg>
                    </div>
                </div>
                <div class="md:w-1/2 mt-8 md:mt-0 text-center md:text-left animate-slide-up">
                    <h1 class="text-4xl md:text-5xl font-bold mb-4">Hello! I'm <span class="text-secondary-light">John Doe</span></h1>
                    <p class="text-xl md:text-2xl mb-6 text-secondary-light opacity-90">Business Professional & Global Talent</p>
                    <p class="text-lg mb-8 max-w-lg mx-auto md:mx-0">A Vietnamese professional with over 3 years of experience living and working in South Korea, connecting cultures and driving innovation.</p>
                    <div class="flex flex-wrap justify-center md:justify-start gap-4">
                        <a href="#contact" class="bg-white text-primary-dark px-6 py-3 rounded-full font-medium hover:bg-secondary-light transition-colors shadow-lg hover:shadow-xl">Contact Me</a>
                        <a href="#projects" class="bg-transparent border-2 border-white px-6 py-3 rounded-full font-medium hover:bg-white hover:text-primary-dark transition-colors">View Projects</a>
                    </div>
                </div>
            </div>
        </div>
        <div class="absolute bottom-0 left-0 w-full overflow-hidden">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320" class="w-full h-auto">
                <path fill="#F9FAFB" fill-opacity="1" d="M0,96L48,112C96,128,192,160,288,160C384,160,480,128,576,122.7C672,117,768,139,864,149.3C960,160,1056,160,1152,138.7C1248,117,1344,75,1392,53.3L1440,32L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path>
            </svg>
        </div>
    </section>

    <!-- About Me -->
    <section id="about" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 gradient-text">About Me</h2>
            <div class="max-w-4xl mx-auto bg-white rounded-xl shadow-custom p-8 animate-fade-in">
                <p class="text-lg leading-relaxed mb-6">
                    Hello! I'm a Vietnamese professional with over 3 years of experience living and working in South Korea. I hold a Master's degree in Business Administration, and I'm passionate about building meaningful connections across cultures.
                </p>
                <p class="text-lg leading-relaxed mb-6">
                    Throughout my career, I've worked in dynamic, multicultural environments—ranging from international education and student affairs to global project coordination and IT solutions. These experiences have sharpened my adaptability, communication skills, and ability to thrive in diverse teams.
                </p>
                <p class="text-lg leading-relaxed">
                    I consider myself a global talent who understands both Korean and Vietnamese business practices, and I'm eager to contribute to forward-thinking organizations that value innovation, inclusivity, and cross-border collaboration.
                </p>
            </div>
        </div>
    </section>

    <!-- Education -->
    <section id="education" class="py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 gradient-text">Education</h2>
            <div class="max-w-4xl mx-auto">
                <div class="bg-white rounded-xl shadow-custom p-6 mb-8 transform transition-all hover:shadow-xl animate-slide-up">
                    <div class="flex flex-col md:flex-row">
                        <div class="md:w-1/4 mb-4 md:mb-0">
                            <div class="gradient-bg text-white text-center py-3 px-4 rounded-lg">
                                <span class="block text-sm">2018 - 2020</span>
                            </div>
                        </div>
                        <div class="md:w-3/4 md:pl-6">
                            <h3 class="text-xl font-bold text-primary-dark mb-2">Master of Business Administration</h3>
                            <h4 class="text-lg font-medium text-gray-700 mb-3">Seoul National University</h4>
                            <p class="text-gray-600">Specialization: International Business</p>
                            <p class="text-gray-600">GPA: 3.8/4.0</p>
                            <p class="text-gray-600 mt-2">Thesis: "Cross-Cultural Business Strategies between Vietnam and South Korea"</p>
                        </div>
                    </div>
                </div>

                <div class="bg-white rounded-xl shadow-custom p-6 transform transition-all hover:shadow-xl animate-slide-up" style="animation-delay: 0.2s">
                    <div class="flex flex-col md:flex-row">
                        <div class="md:w-1/4 mb-4 md:mb-0">
                            <div class="gradient-bg text-white text-center py-3 px-4 rounded-lg">
                                <span class="block text-sm">2014 - 2018</span>
                            </div>
                        </div>
                        <div class="md:w-3/4 md:pl-6">
                            <h3 class="text-xl font-bold text-primary-dark mb-2">Bachelor of International Relations</h3>
                            <h4 class="text-lg font-medium text-gray-700 mb-3">Vietnam National University, Hanoi</h4>
                            <p class="text-gray-600">Specialization: East Asian Studies</p>
                            <p class="text-gray-600">GPA: 3.7/4.0</p>
                            <p class="text-gray-600 mt-2">Graduated with Honors. Participated in student exchange program with Yonsei University.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience -->
    <section id="experience" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 gradient-text">Professional Experience</h2>
            <div class="max-w-4xl mx-auto">
                <div class="relative">
                    <!-- Timeline line -->
                    <div class="hidden md:block absolute left-1/2 transform -translate-x-1/2 h-full w-1 bg-gradient-to-b from-primary to-secondary-dark"></div>
                    
                    <!-- Experience 1 -->
                    <div class="relative mb-12">
                        <div class="hidden md:block absolute left-1/2 transform -translate-x-1/2 -mt-3">
                            <div class="w-6 h-6 rounded-full gradient-bg border-4 border-white shadow"></div>
                        </div>
                        <div class="md:w-1/2 md:pr-8 md:text-right animate-slide-in" style="animation-delay: 0.1s">
                            <div class="bg-white rounded-xl shadow-custom p-6 hover:shadow-xl transition-shadow">
                                <h3 class="text-xl font-bold text-primary-dark mb-2">Global Project Coordinator</h3>
                                <h4 class="text-lg font-medium text-gray-700 mb-2">Samsung Electronics</h4>
                                <div class="text-sm text-primary font-medium mb-3">2020 - Present</div>
                                <ul class="text-gray-600 list-disc list-inside md:list-outside">
                                    <li>Coordinate cross-border projects between Korean headquarters and Vietnamese branch offices</li>
                                    <li>Facilitate communication between multicultural teams, ensuring clear understanding of project goals</li>
                                    <li>Manage stakeholder relationships across different cultural contexts</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Experience 2 -->
                    <div class="relative mb-12 md:mt-24">
                        <div class="hidden md:block absolute left-1/2 transform -translate-x-1/2 -mt-3">
                            <div class="w-6 h-6 rounded-full gradient-bg border-4 border-white shadow"></div>
                        </div>
                        <div class="md:w-1/2 md:ml-auto md:pl-8 animate-slide-in" style="animation-delay: 0.2s">
                            <div class="bg-white rounded-xl shadow-custom p-6 hover:shadow-xl transition-shadow">
                                <h3 class="text-xl font-bold text-primary-dark mb-2">International Student Affairs Officer</h3>
                                <h4 class="text-lg font-medium text-gray-700 mb-2">Korea University</h4>
                                <div class="text-sm text-primary font-medium mb-3">2018 - 2020</div>
                                <ul class="text-gray-600 list-disc list-inside md:list-outside">
                                    <li>Provided support services for international students from Southeast Asia</li>
                                    <li>Organized cultural exchange events and orientation programs</li>
                                    <li>Developed bilingual resources to help students navigate Korean academic environment</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Experience 3 -->
                    <div class="relative md:mt-24">
                        <div class="hidden md:block absolute left-1/2 transform -translate-x-1/2 -mt-3">
                            <div class="w-6 h-6 rounded-full gradient-bg border-4 border-white shadow"></div>
                        </div>
                        <div class="md:w-1/2 md:pr-8 md:text-right animate-slide-in" style="animation-delay: 0.3s">
                            <div class="bg-white rounded-xl shadow-custom p-6 hover:shadow-xl transition-shadow">
                                <h3 class="text-xl font-bold text-primary-dark mb-2">Marketing Intern</h3>
                                <h4 class="text-lg font-medium text-gray-700 mb-2">LG Electronics Vietnam</h4>
                                <div class="text-sm text-primary font-medium mb-3">2017 - 2018</div>
                                <ul class="text-gray-600 list-disc list-inside md:list-outside">
                                    <li>Assisted in market research for product launches in Vietnamese market</li>
                                    <li>Translated marketing materials between Korean, English, and Vietnamese</li>
                                    <li>Supported social media campaigns targeting young Vietnamese consumers</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects -->
    <section id="projects" class="py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 gradient-text">Featured Projects</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Project 1 -->
                <div class="project-card bg-white rounded-xl shadow-custom overflow-hidden animate-fade-in" style="animation-delay: 0.1s">
                    <div class="relative h-48 gradient-bg">
                        <svg class="absolute inset-0 w-full h-full text-white opacity-30" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M4 5a2 2 0 012-2h12a2 2 0 012 2v14a2 2 0 01-2 2H6a2 2 0 01-2-2V5zm3 1h10v4H7V6zm0 6h10v2H7v-2zm0 4h7v2H7v-2z"></path>
                        </svg>
                        <div class="absolute inset-0 flex items-center justify-center">
                            <h3 class="text-xl font-bold text-white">Cross-Cultural Training Program</h3>
                        </div>
                    </div>
                    <div class="p-6">
                        <p class="text-gray-600 mb-4">Developed and implemented a comprehensive training program for Korean executives working with Vietnamese teams, focusing on cultural intelligence and effective communication.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-primary text-white text-xs px-3 py-1 rounded-full">Cultural Intelligence</span>
                            <span class="bg-primary text-white text-xs px-3 py-1 rounded-full">Leadership</span>
                            <span class="bg-primary text-white text-xs px-3 py-1 rounded-full">Training</span>
                        </div>
                        <div class="flex justify-between">
                            <a href="#" class="text-primary hover:text-primary-dark font-medium flex items-center">
                                <span>View Details</span>
                                <i class="fas fa-arrow-right ml-2"></i>
                            </a>
                            <a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ" target="_blank" class="text-primary hover:text-primary-dark font-medium flex items-center">
                                <i class="fab fa-youtube mr-2"></i>
                                <span>Demo</span>
                            </a>
                        </div>
                    </div>
                </div>
                
                <!-- Project 2 -->
                <div class="project-card bg-white rounded-xl shadow-custom overflow-hidden animate-fade-in" style="animation-delay: 0.2s">
                    <div class="relative h-48 gradient-bg">
                        <svg class="absolute inset-0 w-full h-full text-white opacity-30" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1 17.93c-3.95-.49-7-3.85-7-7.93 0-.62.08-1.21.21-1.79L9 15v1c0 1.1.9 2 2 2v1.93zm6.9-2.54c-.26-.81-1-1.39-1.9-1.39h-1v-3c0-.55-.45-1-1-1H8v-2h2c.55 0 1-.45 1-1V7h2c1.1 0 2-.9 2-2v-.41c2.93 1.19 5 4.06 5 7.41 0 2.08-.8 3.97-2.1 5.39z"></path>
                        </svg>
                        <div class="absolute inset-0 flex items-center justify-center">
                            <h3 class="text-xl font-bold text-white">Market Entry Strategy</h3>
                        </div>
                    </div>
                    <div class="p-6">
                        <p class="text-gray-600 mb-4">Led a team developing market entry strategies for Korean tech companies expanding into Vietnam, including competitive analysis and localization recommendations.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-primary text-white text-xs px-3 py-1 rounded-full">Market Research</span>
                            <span class="bg-primary text-white text-xs px-3 py-1 rounded-full">Strategy</span>
                            <span class="bg-primary text-white text-xs px-3 py-1 rounded-full">Business Development</span>
                        </div>
                        <div class="flex justify-between">
                            <a href="#" class="text-primary hover:text-primary-dark font-medium flex items-center">
                                <span>View Details</span>
                                <i class="fas fa-arrow-right ml-2"></i>
                            </a>
                            <a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ" target="_blank" class="text-primary hover:text-primary-dark font-medium flex items-center">
                                <i class="fab fa-youtube mr-2"></i>
                                <span>Demo</span>
                            </a>
                        </div>
                    </div>
                </div>
                
                <!-- Project 3 -->
                <div class="project-card bg-white rounded-xl shadow-custom overflow-hidden animate-fade-in" style="animation-delay: 0.3s">
                    <div class="relative h-48 gradient-bg">
                        <svg class="absolute inset-0 w-full h-full text-white opacity-30" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M19 3H5c-1.1 0-2 .9-2 2v14c0 1.1.9 2 2 2h14c1.1 0 2-.9 2-2V5c0-1.1-.9-2-2-2zm-5 14h-2V9h-2V7h4v10z"></path>
                        </svg>
                        <div class="absolute inset-0 flex items-center justify-center">
                            <h3 class="text-xl font-bold text-white">Bilingual Education Platform</h3>
                        </div>
                    </div>
                    <div class="p-6">
                        <p class="text-gray-600 mb-4">Designed and launched an online platform connecting Korean language learners with Vietnamese students learning Korean, featuring interactive lessons and cultural exchange opportunities.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-primary text-white text-xs px-3 py-1 rounded-full">EdTech</span>
                            <span class="bg-primary text-white text-xs px-3 py-1 rounded-full">Language Learning</span>
                            <span class="bg-primary text-white text-xs px-3 py-1 rounded-full">Cultural Exchange</span>
                        </div>
                        <div class="flex justify-between">
                            <a href="#" class="text-primary hover:text-primary-dark font-medium flex items-center">
                                <span>View Details</span>
                                <i class="fas fa-arrow-right ml-2"></i>
                            </a>
                            <a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ" target="_blank" class="text-primary hover:text-primary-dark font-medium flex items-center">
                                <i class="fab fa-youtube mr-2"></i>
                                <span>Demo</span>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills -->
    <section id="skills" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 gradient-text">Skills & Expertise</h2>
            
            <div class="max-w-4xl mx-auto">
                <!-- Professional Skills -->
                <div class="mb-12 animate-slide-up">
                    <h3 class="text-2xl font-bold text-primary mb-6">Professional Skills</h3>
                    <div class="flex flex-wrap gap-3">
                        <span class="skill-pill bg-primary-dark text-white px-4 py-2 rounded-full text-sm font-medium">Cross-Cultural Communication</span>
                        <span class="skill-pill bg-primary text-white px-4 py-2 rounded-full text-sm font-medium">Project Management</span>
                        <span class="skill-pill bg-primary-light text-white px-4 py-2 rounded-full text-sm font-medium">Business Development</span>
                        <span class="skill-pill bg-primary-dark text-white px-4 py-2 rounded-full text-sm font-medium">Market Research</span>
                        <span class="skill-pill bg-primary text-white px-4 py-2 rounded-full text-sm font-medium">Strategic Planning</span>
                        <span class="skill-pill bg-primary-light text-white px-4 py-2 rounded-full text-sm font-medium">International Relations</span>
                        <span class="skill-pill bg-primary-dark text-white px-4 py-2 rounded-full text-sm font-medium">Cultural Intelligence</span>
                        <span class="skill-pill bg-primary text-white px-4 py-2 rounded-full text-sm font-medium">Stakeholder Management</span>
                        <span class="skill-pill bg-primary-light text-white px-4 py-2 rounded-full text-sm font-medium">Public Speaking</span>
                    </div>
                </div>
                
                <!-- Languages -->
                <div class="mb-12 animate-slide-up" style="animation-delay: 0.2s">
                    <h3 class="text-2xl font-bold text-primary mb-6">Languages</h3>
                    <div class="space-y-4">
                        <div>
                            <div class="flex justify-between mb-1">
                                <span class="font-medium">Vietnamese</span>
                                <span>Native</span>
                            </div>
                            <div class="w-full bg-gray-200 rounded-full h-2">
                                <div class="gradient-bg h-2 rounded-full" style="width: 100%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-1">
                                <span class="font-medium">English</span>
                                <span>Fluent (C1)</span>
                            </div>
                            <div class="w-full bg-gray-200 rounded-full h-2">
                                <div class="gradient-bg h-2 rounded-full" style="width: 90%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-1">
                                <span class="font-medium">Korean</span>
                                <span>Advanced (B2)</span>
                            </div>
                            <div class="w-full bg-gray-200 rounded-full h-2">
                                <div class="gradient-bg h-2 rounded-full" style="width: 75%"></div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Soft Skills -->
                <div class="animate-slide-up" style="animation-delay: 0.3s">
                    <h3 class="text-2xl font-bold text-primary mb-6">Soft Skills</h3>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <div class="bg-white p-4 rounded-lg shadow-custom">
                            <div class="flex items-center">
                                <div class="w-12 h-12 gradient-bg rounded-full flex items-center justify-center text-white">
                                    <i class="fas fa-users text-xl"></i>
                                </div>
                                <div class="ml-4">
                                    <h4 class="font-bold">Teamwork</h4>
                                    <div class="flex mt-1">
                                        <i class="fas fa-star text-yellow-500"></i>
                                        <i class="fas fa-star text-yellow-500"></i>
                                        <i class="fas fa-star text-yellow-500"></i>
                                        <i class="fas fa-star text-yellow-500"></i>
                                        <i class="fas fa-star text-yellow-500"></i>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="bg-white p-4 rounded-lg shadow-custom">
                            <div class="flex items-center">
                                <div class="w-12 h-12 gradient-bg rounded-full flex items-center justify-center text-white">
                                    <i class="fas fa-comments text-xl"></i>
                                </div>
                                <div class="ml-4">
                                    <h4 class="font-bold">Communication</h4>
                                    <div class="flex mt-1">
                                        <i class="fas fa-star text-yellow-500"></i>
                                        <i class="fas fa-star text-yellow-500"></i>
                                        <i class="fas fa-star text-yellow-500"></i>
                                        <i class="fas fa-star text-yellow-500"></i>
                                        <i class="fas fa-star-half-alt text-yellow-500"></i>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="bg-white p-4 rounded-lg shadow-custom">
                            <div class="flex items-center">
                                <div class="w-12 h-12 gradient-bg rounded-full flex items-center justify-center text-white">
                                    <i class="fas fa-lightbulb text-xl"></i>
                                </div>
                                <div class="ml-4">
                                    <h4 class="font-bold">Problem Solving</h4>
                                    <div class="flex mt-1">
                                        <i class="fas fa-star text-yellow-500"></i>
                                        <i class="fas fa-star text-yellow-500"></i>
                                        <i class="fas fa-star text-yellow-500"></i>
                                        <i class="fas fa-star text-yellow-500"></i>
                                        <i class="fas fa-star text-yellow-500"></i>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="bg-white p-4 rounded-lg shadow-custom">
                            <div class="flex items-center">
                                <div class="w-12 h-12 gradient-bg rounded-full flex items-center justify-center text-white">
                                    <i class="fas fa-tasks text-xl"></i>
                                </div>
                                <div class="ml-4">
                                    <h4 class="font-bold">Adaptability</h4>
                                    <div class="flex mt-1">
                                        <i class="fas fa-star text-yellow-500"></i>
                                        <i class="fas fa-star text-yellow-500"></i>
                                        <i class="fas fa-star text-yellow-500"></i>
                                        <i class="fas fa-star text-yellow-500"></i>
                                        <i class="fas fa-star text-yellow-500"></i>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact -->
    <section id="contact" class="py-16 bg-gradient-to-br from-dark-dark via-primary-dark to-primary text-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12">Get In Touch</h2>
            
            <div class="max-w-4xl mx-auto bg-white rounded-xl shadow-xl p-8 text-gray-800">
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                    <div class="animate-fade-in">
                        <h3 class="text-2xl font-bold gradient-text mb-6">Contact Information</h3>
                        <div class="space-y-4">
                            <div class="flex items-center">
                                <div class="w-10 h-10 rounded-full gradient-bg flex items-center justify-center text-white">
                                    <i class="fas fa-envelope"></i>
                                </div>
                                <div class="ml-4">
                                    <p class="text-sm text-gray-500">Email</p>
                                    <p class="font-medium">john.doe@example.com</p>
                                </div>
                            </div>
                            <div class="flex items-center">
                                <div class="w-10 h-10 rounded-full gradient-bg flex items-center justify-center text-white">
                                    <i class="fas fa-phone"></i>
                                </div>
                                <div class="ml-4">
                                    <p class="text-sm text-gray-500">Phone</p>
                                    <p class="font-medium">+82 10 1234 5678</p>
                                </div>
                            </div>
                            <div class="flex items-center">
                                <div class="w-10 h-10 rounded-full gradient-bg flex items-center justify-center text-white">
                                    <i class="fas fa-map-marker-alt"></i>
                                </div>
                                <div class="ml-4">
                                    <p class="text-sm text-gray-500">Location</p>
                                    <p class="font-medium">Seoul, South Korea</p>
                                </div>
                            </div>
                        </div>
                        
                        <div class="mt-8">
                            <h4 class="font-bold mb-4">Connect With Me</h4>
                            <div class="flex space-x-4">
                                <a href="#" class="w-10 h-10 rounded-full bg-blue-600 flex items-center justify-center text-white hover:bg-blue-700 transition-colors">
                                    <i class="fab fa-facebook-f"></i>
                                </a>
                                <a href="#" class="w-10 h-10 rounded-full bg-blue-400 flex items-center justify-center text-white hover:bg-blue-500 transition-colors">
                                    <i class="fab fa-twitter"></i>
                                </a>
                                <a href="#" class="w-10 h-10 rounded-full bg-blue-700 flex items-center justify-center text-white hover:bg-blue-800 transition-colors">
                                    <i class="fab fa-linkedin-in"></i>
                                </a>
                                <a href="#" class="w-10 h-10 rounded-full bg-gray-800 flex items-center justify-center text-white hover:bg-black transition-colors">
                                    <i class="fab fa-github"></i>
                                </a>
                            </div>
                        </div>
                    </div>
                    
                    <div class="animate-slide-up">
                        <h3 class="text-2xl font-bold gradient-text mb-6">Send Me a Message</h3>
                        <form class="space-y-4">
                            <div>
                                <label for="name" class="block text-sm font-medium text-gray-700 mb-1">Full Name</label>
                                <input type="text" id="name" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-primary outline-none transition-colors" placeholder="Enter your full name">
                            </div>
                            <div>
                                <label for="email" class="block text-sm font-medium text-gray-700 mb-1">Email</label>
                                <input type="email" id="email" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-primary outline-none transition-colors" placeholder="Enter your email address">
                            </div>
                            <div>
                                <label for="message" class="block text-sm font-medium text-gray-700 mb-1">Message</label>
                                <textarea id="message" rows="4" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-primary outline-none transition-colors" placeholder="Enter your message"></textarea>
                            </div>
                            <button type="button" class="w-full gradient-bg text-white font-medium py-3 px-6 rounded-lg hover:opacity-90 transition-opacity focus:outline-none focus:ring-2 focus:ring-primary focus:ring-offset-2">
                                Send Message
                            </button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-dark-dark text-white py-8">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="mb-4 md:mb-0">
                    <h2 class="text-2xl font-bold">John Doe</h2>
                    <p class="text-gray-400">Business Professional & Global Talent</p>
                </div>
                <div class="flex space-x-4">
                    <a href="#" class="hover:text-primary-light transition-colors">
                        <i class="fab fa-facebook-f"></i>
                    </a>
                    <a href="#" class="hover:text-primary-light transition-colors">
                        <i class="fab fa-twitter"></i>
                    </a>
                    <a href="#" class="hover:text-primary-light transition-colors">
                        <i class="fab fa-linkedin-in"></i>
                    </a>
                    <a href="#" class="hover:text-primary-light transition-colors">
                        <i class="fab fa-github"></i>
                    </a>
                </div>
            </div>
            <div class="mt-6 text-center text-gray-400 text-sm">
                <p>&copy; 2023 John Doe. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');
        
        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
        
        // Navigation active state
        const sections = document.querySelectorAll('section');
        const navLinks = document.querySelectorAll('.nav-link');
        
        window.addEventListener('scroll', () => {
            let current = '';
            
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.clientHeight;
                if (pageYOffset >= (sectionTop - sectionHeight / 3)) {
                    current = section.getAttribute('id');
                }
            });
            
            navLinks.forEach(link => {
                link.classList.remove('active');
                if (link.getAttribute('href').substring(1) === current) {
                    link.classList.add('active');
                }
            });
        });
        
        // Form submission (demo)
        const contactForm = document.querySelector('form');
        const submitButton = contactForm.querySelector('button');
        
        submitButton.addEventListener('click', (e) => {
            e.preventDefault();
            const nameInput = document.getElementById('name');
            const emailInput = document.getElementById('email');
            const messageInput = document.getElementById('message');
            
            if (nameInput.value && emailInput.value && messageInput.value) {
                submitButton.innerHTML = '<i class="fas fa-check mr-2"></i> Message Sent!';
                submitButton.classList.add('bg-green-600');
                submitButton.classList.remove('gradient-bg', 'hover:opacity-90');
                
                // Reset form
                setTimeout(() => {
                    nameInput.value = '';
                    emailInput.value = '';
                    messageInput.value = '';
                    submitButton.innerHTML = 'Send Message';
                    submitButton.classList.remove('bg-green-600');
                    submitButton.classList.add('gradient-bg', 'hover:opacity-90');
                }, 3000);
            } else {
                alert('Please fill in all fields!');
            }
        });
        
        // Animate elements on scroll
        const animateElements = document.querySelectorAll('.animate-fade-in, .animate-slide-up, .animate-slide-in');
        
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0) translateX(0)';
                }
            });
        }, { threshold: 0.1 });
        
        animateElements.forEach(element => {
            element.style.opacity = '0';
            if (element.classList.contains('animate-slide-up')) {
                element.style.transform = 'translateY(50px)';
            } else if (element.classList.contains('animate-slide-in')) {
                element.style.transform = 'translateX(-50px)';
            }
            element.style.transition = 'opacity 0.8s ease, transform 0.8s ease';
            observer.observe(element);
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9630332e1173ea18',t:'MTc1MzE1ODU5Ny4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
