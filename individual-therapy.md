<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Individual Therapy | TLC Family Services</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@500;600;700&family=Lato:wght@300;400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        .font-serif {
            font-family: 'Cormorant Garamond', serif;
        }
        .font-sans {
            font-family: 'Lato', sans-serif;
        }
        .wavy-divider {
            background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 1200 120' preserveAspectRatio='none'%3E%3Cpath d='M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z' fill='%23C7B8E3'%3E%3C/path%3E%3C/svg%3E");
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
        }
        .bg-watercolor {
            background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='100%25' height='100%25' viewBox='0 0 800 800'%3E%3Cg %3E%3Ccircle fill='%23C7B8E3' cx='400' cy='400' r='600'/%3E%3Ccircle fill='%23B0C4DE' cx='400' cy='400' r='500'/%3E%3Ccircle fill='%23C7B8E3' cx='400' cy='400' r='400'/%3E%3Ccircle fill='%23FFB6C1' cx='400' cy='400' r='300'/%3E%3Ccircle fill='%23B0C4DE' cx='400' cy='400' r='200'/%3E%3Ccircle fill='%23C7B8E3' cx='400' cy='400' r='100'/%3E%3C/g%3E%3C/svg%3E");
            background-attachment: fixed;
            background-size: cover;
            background-position: center;
            opacity: 0.1;
        }
        .modal {
            display: none;
            position: fixed;
            z-index: 50;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgba(0,0,0,0.4);
        }
        .modal-content {
            background-color: #fefefe;
            margin: 15% auto;
            padding: 20px;
            border: 1px solid #888;
            width: 80%;
            max-width: 500px;
            border-radius: 8px;
        }
        .close {
            color: #aaa;
            float: right;
            font-size: 28px;
            font-weight: bold;
        }
        .close:hover,
        .close:focus {
            color: black;
            text-decoration: none;
            cursor: pointer;
        }
        .accordion-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease;
        }
        .accordion-content.open {
            max-height: 1000px;
        }
    </style>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        purple: {
                            50: '#f9f8fc',
                            100: '#f3f1f9',
                            200: '#e9e3f4',
                            300: '#d9d0ed',
                            400: '#c7b8e3',
                            500: '#b39cd6',
                            600: '#9f81c9',
                            700: '#8a65b9',
                            800: '#744ba5',
                            900: '#5f368e',
                            950: '#48226d',
                        },
                        pink: {
                            50: '#fdf4f7',
                            100: '#fce8ef',
                            200: '#fad0df',
                            300: '#f7b2cb',
                            400: '#ffb6c1',
                            500: '#f47ca0',
                            600: '#e95f86',
                            700: '#dd436e',
                            800: '#c92c59',
                            900: '#a91f48',
                            950: '#870f37',
                        },
                        blue: {
                            50: '#f4f8fa',
                            100: '#e9f0f5',
                            200: '#d7e2ea',
                            300: '#c0d0de',
                            400: '#b0c4de',
                            500: '#92a8c9',
                            600: '#758cb3',
                            700: '#5c729d',
                            800: '#475a82',
                            900: '#35446a',
                            950: '#222c4a',
                        },
                        yellow: {
                            50: '#fffdf5',
                            100: '#fffbeb',
                            200: '#fff7d6',
                            300: '#fff2c1',
                            400: '#fffacd',
                            500: '#f5e9a3',
                            600: '#ebd97a',
                            700: '#e1c851',
                            800: '#d7b728',
                            900: '#cda600',
                            950: '#a38300',
                        }
                    }
                }
            }
        }
    </script>
</head>
<body class="font-sans text-purple-900 bg-white">
    <!-- Navigation -->
    <nav class="bg-white shadow-sm sticky top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-16">
                <div class="flex items-center">
                    <div class="flex-shrink-0 flex items-center">
                        <img src='https://i.postimg.cc/ncrCsgHY/tlc-logo.png' alt='tlc-logo' class="h-10 w-10">
                        <span class="ml-2 font-serif text-xl font-bold text-purple-700">TLC Family Services</span>
                    </div>
                </div>
                <div class="hidden md:ml-6 md:flex md:items-center md:space-x-8">
                    <a href="index.html#home" class="px-3 py-2 text-sm font-medium text-purple-900 border-b-2 border-transparent hover:border-purple-500">Home</a>
                    <a href="index.html#services" class="px-3 py-2 text-sm font-medium text-purple-900 border-b-2 border-transparent hover:border-purple-500">Services</a>
                    <a href="index.html#resources" class="px-3 py-2 text-sm font-medium text-purple-900 border-b-2 border-transparent hover:border-purple-500">Resources</a>
                    <a href="index.html#events" class="px-3 py-2 text-sm font-medium text-purple-900 border-b-2 border-transparent hover:border-purple-500">Events</a>
                    <a href="index.html#about" class="px-3 py-2 text-sm font-medium text-purple-900 border-b-2 border-transparent hover:border-purple-500">About Us</a>
                    <a href="#" onclick="openEmail()" class="inline-flex items-center px-4 py-2 border border-transparent text-sm font-medium rounded-md shadow-sm text-white bg-purple-600 hover:bg-purple-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-purple-500">
                        Contact Us
                    </a>
                </div>
                <div class="-mr-2 flex items-center md:hidden">
                    <button type="button" id="mobile-menu-button" class="inline-flex items-center justify-center p-2 rounded-md text-purple-400 hover:text-purple-500 hover:bg-purple-100 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-purple-500">
                        <span class="sr-only">Open main menu</span>
                        <i class="fas fa-bars"></i>
                    </button>
                </div>
            </div>
        </div>
        <!-- Mobile menu -->
        <div class="hidden md:hidden" id="mobile-menu">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3 bg-white">
                <a href="index.html#home" class="text-purple-900 hover:text-purple-700 block px-3 py-2 rounded-md text-base font-medium">Home</a>
                <a href="index.html#services" class="text-purple-900 hover:text-purple-700 block px-3 py-2 rounded-md text-base font-medium">Services</a>
                <a href="index.html#resources" class="text-purple-900 hover:text-purple-700 block px-3 py-2 rounded-md text-base font-medium">Resources</a>
                <a href="index.html#events" class="text-purple-900 hover:text-purple-700 block px-3 py-2 rounded-md text-base font-medium">Events</a>
                <a href="index.html#about" class="text-purple-900 hover:text-purple-700 block px-3 py-2 rounded-md text-base font-medium">About Us</a>
                <a href="#" onclick="openEmail()" class="bg-purple-600 hover:bg-purple-700 text-white block px-3 py-2 rounded-md text-base font-medium transition duration-300">Contact Us</a>
            </div>
        </div>
    </nav>
    <!-- Hero Section -->
    <section class="relative bg-blue-50 overflow-hidden">
        <div class="absolute inset-0 bg-watercolor"></div>
        <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-20 md:py-32 text-center">
            <h1 class="font-serif text-4xl md:text-5xl font-bold text-purple-800 mb-6 leading-tight">
                Individual Therapy: Your Path to Personal Growth
            </h1>
            <div class="w-24 h-1 bg-purple-500 mx-auto mb-8"></div>
            <p class="text-xl text-pink-700 max-w-3xl mx-auto">
                Compassionate one-on-one support tailored to your unique journey through life's challenges.
            </p>
        </div>
        <div class="wavy-divider h-16 -mt-8"></div>
    </section>
    <!-- Therapy Approach -->
    <section class="py-16 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="lg:grid lg:grid-cols-2 lg:gap-16 items-center">
                <div class="mb-12 lg:mb-0">
                    <div class="relative rounded-lg shadow-xl overflow-hidden">
                        <img src="https://images.pexels.com/photos/4173234/pexels-photo-4173234.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="Lonely individual reflecting" class="w-full h-auto object-cover" loading="lazy">
                        <div class="absolute inset-0 bg-gradient-to-t from-black/30 to-transparent"></div>
                        <div class="absolute bottom-0 left-0 p-6 text-white">
                            <p class="font-serif italic">"Healing begins with being heard."</p>
                        </div>
                    </div>
                </div>
                <div>
                    <h2 class="font-serif text-3xl font-bold text-purple-800 mb-6">
                        Our Individual Therapy Approach
                    </h2>
                    <p class="text-pink-700 mb-6">
                        At TLC Family Services, we believe every individual's healing journey is unique. Our therapists blend evidence-based techniques with personalized care to help you:
                    </p>
                    <ul class="space-y-4 mb-8">
                        <li class="flex items-start">
                            <div class="flex-shrink-0 h-6 w-6 text-purple-600 mt-1 mr-3">
                                <i class="fas fa-leaf"></i>
                            </div>
                            <p class="text-pink-700">
                                <strong class="text-purple-800">Develop coping tools</strong> for anxiety, depression, or life transitions
                            </p>
                        </li>
                        <li class="flex items-start">
                            <div class="flex-shrink-0 h-6 w-6 text-purple-600 mt-1 mr-3">
                                <i class="fas fa-leaf"></i>
                            </div>
                            <p class="text-pink-700">
                                <strong class="text-purple-800">Build resilience</strong> through strength-based strategies
                            </p>
                        </li>
                        <li class="flex items-start">
                            <div class="flex-shrink-0 h-6 w-6 text-purple-600 mt-1 mr-3">
                                <i class="fas fa-leaf"></i>
                            </div>
                            <p class="text-pink-700">
                                <strong class="text-purple-800">Navigate challenges</strong> at any life stage (ages 5-60+)
                            </p>
                        </li>
                    </ul>
                    <a href="index.html#resources" class="inline-block bg-purple-600 text-white font-medium px-8 py-3 rounded-lg hover:bg-purple-700 transition duration-300">
                        Start Your Journey
                    </a>
                </div>
            </div>
        </div>
    </section>
    <!-- Who We Help -->
    <section class="py-16 bg-purple-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="font-serif text-3xl font-bold text-purple-800 mb-12">
                Specialized Support Across All Ages
            </h2>
            <div class="grid md:grid-cols-3 gap-8">
                <!-- Children -->
                <div class="bg-white p-8 rounded-lg shadow-sm hover:shadow-md transition duration-300">
                    <div class="text-purple-600 text-4xl mb-4">
                        <i class="fas fa-child"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold text-purple-800 mb-3">
                        Children (5-12)
                    </h3>
                    <p class="text-pink-700 mb-4">
                        Play therapy and creative techniques to help young minds express emotions and build confidence.
                    </p>
                    <div class="text-sm text-purple-600">
                        Common focuses: Anxiety • ADHD • School struggles
                    </div>
                </div>
                
                <!-- Adolescents -->
                <div class="bg-white p-8 rounded-lg shadow-sm hover:shadow-md transition duration-300">
                    <div class="text-purple-600 text-4xl mb-4">
                        <i class="fas fa-user-graduate"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold text-purple-800 mb-3">
                        Adolescents (13-19)
                    </h3>
                    <p class="text-pink-700 mb-4">
                        Safe space to navigate identity, relationships, and the transition to adulthood.
                    </p>
                    <div class="text-sm text-purple-600">
                        Common focuses: Depression • Self-esteem • Social stress
                    </div>
                </div>
                
                <!-- Adults -->
                <div class="bg-white p-8 rounded-lg shadow-sm hover:shadow-md transition duration-300">
                    <div class="text-purple-600 text-4xl mb-4">
                        <i class="fas fa-user-tie"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold text-purple-800 mb-3">
                        Adults (20+)
                    </h3>
                    <p class="text-pink-700 mb-4">
                        Evidence-based approaches for life transitions, trauma, and personal growth.
                    </p>
                    <div class="text-sm text-purple-600">
                        Common focuses: Anxiety • Career stress • Relationships
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- Techniques -->
    <section class="py-16 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="font-serif text-3xl font-bold text-purple-800 mb-6">
                Therapeutic Techniques We Use
            </h2>
            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
                <div class="border border-purple-200 rounded-lg p-6 text-center hover:bg-purple-50 transition duration-300">
                    <div class="text-purple-600 text-3xl mb-4">
                        <i class="fas fa-brain"></i>
                    </div>
                    <h3 class="font-serif text-lg font-bold text-purple-800 mb-2">CBT</h3>
                    <p class="text-pink-700 text-sm">
                        Cognitive Behavioral Therapy to reframe negative thought patterns
                    </p>
                </div>
                
                <div class="border border-purple-200 rounded-lg p-6 text-center hover:bg-purple-50 transition duration-300">
                    <div class="text-purple-600 text-3xl mb-4">
                        <i class="fas fa-heart"></i>
                    </div>
                    <h3 class="font-serif text-lg font-bold text-purple-800 mb-2">Mindfulness</h3>
                    <p class="text-pink-700 text-sm">
                        Grounding techniques to manage stress and anxiety
                    </p>
                </div>
                
                <div class="border border-purple-200 rounded-lg p-6 text-center hover:bg-purple-50 transition duration-300">
                    <div class="text-purple-600 text-3xl mb-4">
                        <i class="fas fa-paint-brush"></i>
                    </div>
                    <h3 class="font-serif text-lg font-bold text-purple-800 mb-2">Expressive Arts</h3>
                    <p class="text-pink-700 text-sm">
                        Creative expression for emotional exploration
                    </p>
                </div>
                
                <div class="border border-purple-200 rounded-lg p-6 text-center hover:bg-purple-50 transition duration-300">
                    <div class="text-purple-600 text-3xl mb-4">
                        <i class="fas fa-comments"></i>
                    </div>
                    <h3 class="font-serif text-lg font-bold text-purple-800 mb-2">
                        Talk Therapy
                    </h3>
                    <p class="text-pink-700 text-sm">
                        Supportive dialogue to process life experiences
                    </p>
                </div>
            </div>
        </div>
    </section>
    <!-- FAQ Section -->
    <section class="py-16 bg-purple-50">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12">
                <h2 class="font-serif text-3xl font-bold text-purple-800 mb-6">
                    Frequently Asked Questions
                </h2>
            </div>
            <div class="space-y-4">
                <!-- FAQ Item 1 -->
                <div class="border border-purple-200 rounded-lg overflow-hidden">
                    <button class="w-full flex justify-between items-center p-6 text-left focus:outline-none" onclick="toggleFAQ(1)">
                        <h3 class="font-serif text-lg font-bold text-purple-800">
                            How do I know if therapy is right for me?
                        </h3>
                        <i class="fas fa-chevron-down text-purple-600 transition-transform duration-300" id="faq-icon-1"></i>
                    </button>
                    <div class="accordion-content" id="faq-content-1">
                        <div class="px-6 pb-6 pt-0 text-pink-700">
                            <p>Therapy can benefit anyone facing emotional challenges, life transitions, or simply seeking personal growth. If you're experiencing persistent sadness, anxiety, relationship difficulties, or feel "stuck" in patterns that no longer serve you, therapy can help. Many clients report feeling better after just a few sessions.</p>
                        </div>
                    </div>
                </div>
                
                <!-- FAQ Item 2 -->
                <div class="border border-purple-200 rounded-lg overflow-hidden">
                    <button class="w-full flex justify-between items-center p-6 text-left focus:outline-none" onclick="toggleFAQ(2)">
                        <h3 class="font-serif text-lg font-bold text-purple-800">
                            What can I expect in my first session?
                        </h3>
                        <i class="fas fa-chevron-down text-purple-600 transition-transform duration-300" id="faq-icon-2"></i>
                    </button>
                    <div class="accordion-content" id="faq-content-2">
                        <div class="px-6 pb-6 pt-0 text-pink-700">
                            <p>Your first session is about building comfort and understanding your needs. We'll discuss what brought you to therapy, your history, and goals. There's no pressure to share everything at once - we move at your pace. Many clients feel relieved after the first session simply from being heard.</p>
                        </div>
                    </div>
                </div>
                
                <!-- FAQ Item 3 -->
                <div class="border border-purple-200 rounded-lg overflow-hidden">
                    <button class="w-full flex justify-between items-center p-6 text-left focus:outline-none" onclick="toggleFAQ(3)">
                        <h3 class="font-serif text-lg font-bold text-purple-800">
                            How long does therapy typically last?
                        </h3>
                        <i class="fas fa-chevron-down text-purple-600 transition-transform duration-300" id="faq-icon-3"></i>
                    </button>
                    <div class="accordion-content" id="faq-content-3">
                        <div class="px-6 pb-6 pt-0 text-pink-700">
                            <p>Duration varies based on individual needs. Some clients achieve their goals in 8-12 sessions, while others benefit from longer-term support. We regularly check in on progress and adjust as needed. Most clients attend weekly at first, then transition to biweekly or monthly as they improve.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- Testimonials -->
    <section class="py-16 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12">
                <h2 class="font-serif text-3xl font-bold text-purple-800 mb-6">
                    Client Experiences
                </h2>
            </div>
            <div class="grid md:grid-cols-3 gap-8">
                <!-- Testimonial 1 -->
                <div class="testimonial-card bg-white p-8 rounded-lg shadow-md border border-purple-100 hover:border-purple-200">
                    <div class="flex items-center mb-4">
                        <div class="text-purple-600 text-2xl mr-3">
                            <i class="fas fa-quote-left"></i>
                        </div>
                        <div class="text-pink-700 italic">
                            "Working with my therapist helped me develop tools to manage my anxiety that I use every day."
                        </div>
                    </div>
                    <div class="flex items-center">
                        <div class="h-10 w-10 rounded-full bg-purple-100 flex items-center justify-center text-purple-600 mr-4">
                            <i class="fas fa-user"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-purple-800">Sarah, 28</h4>
                            <p class="text-sm text-pink-600">Anxiety Management</p>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 2 -->
                <div class="testimonial-card bg-white p-8 rounded-lg shadow-md border border-purple-100 hover:border-purple-200">
                    <div class="flex items-center mb-4">
                        <div class="text-purple-600 text-2xl mr-3">
                            <i class="fas fa-quote-left"></i>
                        </div>
                        <div class="text-pink-700 italic">
                            "My son looks forward to his sessions. The play therapy approach has made all the difference."
                        </div>
                    </div>
                    <div class="flex items-center">
                        <div class="h-10 w-10 rounded-full bg-purple-100 flex items-center justify-center text-purple-600 mr-4">
                            <i class="fas fa-user"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-purple-800">Michael, Parent</h4>
                            <p class="text-sm text-pink-600">Child Therapy</p>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 3 -->
                <div class="testimonial-card bg-white p-8 rounded-lg shadow-md border border-purple-100 hover:border-purple-200">
                    <div class="flex items-center mb-4">
                        <div class="text-purple-600 text-2xl mr-3">
                            <i class="fas fa-quote-left"></i>
                        </div>
                        <div class="text-pink-700 italic">
                            "After just a few months, I feel like I have my life back. The mindfulness techniques changed everything."
                        </div>
                    </div>
                    <div class="flex items-center">
                        <div class="h-10 w-10 rounded-full bg-purple-100 flex items-center justify-center text-purple-600 mr-4">
                            <i class="fas fa-user"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-purple-800">James, 42</h4>
                            <p class="text-sm text-pink-600">Stress Management</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- CTA -->
    <section class="py-16 bg-purple-800 text-white">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="font-serif text-3xl font-bold mb-6">
                Ready to Prioritize Your Mental Health?
            </h2>
            <div class="flex flex-col sm:flex-row justify-center gap-4">
                <a href="index.html#resources" class="px-8 py-3 rounded-lg bg-pink-500 hover:bg-pink-600 text-white font-medium transition duration-300 transform hover:scale-105">
                    Schedule a Session
                </a>
                <a href="#" onclick="openCallPopup()" class="px-8 py-3 rounded-lg border-2 border-white hover:bg-white hover:text-purple-800 font-medium transition duration-300"><i class="fas fa-phone mr-2"></i> Call Now</a>
            </div>
        </div>
    </section>
    <!-- Footer -->
    <footer class="bg-purple-900 text-white py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div>
                    <h3 class="font-serif text-xl font-bold mb-4">TLC Family Services</h3>
                    <p class="text-purple-200">
                        Providing compassionate therapy and support for individuals and families.
                    </p>
                </div>
                <div>
                    <h3 class="font-serif text-xl font-bold mb-4">Quick Links</h3>
                    <ul class="space-y-2">
                        <li><a href="index.html#home" class="text-purple-200 hover:text-white">Home</a></li>
                        <li><a href="index.html#services" class="text-purple-200 hover:text-white">Services</a></li>
                        <li><a href="index.html#resources" class="text-purple-200 hover:text-white">Resources</a></li>
                        <li><a href="index.html#events" class="text-purple-200 hover:text-white">Events</a></li>
                        <li><a href="index.html#about" class="text-purple-200 hover:text-white">About Us</a></li>
                    </ul>
                </div>
                <div>
                    <h3 class="font-serif text-xl font-bold mb-4">Contact Info</h3>
                    <p class="text-purple-200">Email: info@tlcfamilyservices.com</p>
                    <p class="text-purple-200">Phone: (123) 456-7890</p>
                    <p class="text-purple-200">Address: 123 Healing Way, Wellness City, MD</p>
                </div>
            </div>
            <div class="mt-8 text-center text-purple-200">
                <p>&copy; 2025 TLC Family Services. All rights reserved.</p>
            </div>
        </div>
    </footer>
    <!-- Contact Modal -->
    <div id="contactModal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <h2 class="font-serif text-2xl font-bold text-purple-800 mb-4">Contact Us</h2>
            <form id="contactForm" class="space-y-4">
                <div>
                    <label for="name" class="block text-sm font-medium text-purple-800">Name</label>
                    <input type="text" id="name" name="name" class="mt-1 block w-full rounded-md border-purple-300 shadow-sm focus:border-purple-500 focus:ring-purple-500">
                </div>
                <div>
                    <label for="email" class="block text-sm font-medium text-purple-800">Email</label>
                    <input type="email" id="email" name="email" class="mt-1 block w-full rounded-md border-purple-300 shadow-sm focus:border-purple-500 focus:ring-purple-500">
                </div>
                <div>
                    <label for="message" class="block text-sm font-medium text-purple-800">Message</label>
                    <textarea id="message" name="message" rows="4" class="mt-1 block w-full rounded-md border-purple-300 shadow-sm focus:border-purple-500 focus:ring-purple-500"></textarea>
                </div>
                <button type="submit" class="w-full bg-purple-600 text-white font-medium px-4 py-2 rounded-md hover:bg-purple-700 transition duration-300">Send Message</button>
            </form>
        </div>
    </div>
    <!-- Call Popup Modal -->
    <div id="call-modal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <h3 class="font-serif text-2xl font-bold text-purple-800 mb-6">Call Us</h3>
            <p class="text-pink-700 text-center">667-355-2334</p>
        </div>
    </div>
    <!-- Privacy Policy Modal -->
    <div id="privacy-modal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <h3 class="font-serif text-2xl font-bold text-purple-800 mb-6">Privacy Policy</h3>
            <p class="text-pink-700">
                At TLC Family Services, your privacy is our priority. In compliance with U.S. health laws like HIPAA, we safeguard your personal health information (PHI) with encrypted storage and secure communications. We only share data with your consent for treatment, payment, or operations. You have rights to access, amend, or restrict your information. We never sell data and use it only for care delivery. For full details, contact us.
            </p>
        </div>
    </div>
    <!-- Terms of Service Modal -->
    <div id="terms-modal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <h3 class="font-serif text-2xl font-bold text-purple-800 mb-6">Terms of Service</h3>
            <p class="text-pink-700">
                By using TLC Family Services, you agree to our terms. We provide virtual therapy in compliance with U.S. health regulations, including confidentiality under HIPAA. Services are for informational and therapeutic purposes; not for emergencies (call 911 or 988). Payment terms: Sessions are billed per agreement; cancellations require 24-hour notice or fees apply. We reserve the right to terminate services if guidelines aren't followed.
            </p>
        </div>
    </div>
    <script>
        // Mobile menu toggle
        document.getElementById('mobile-menu-button').addEventListener('click', function() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        });
        // Accordion toggle for FAQ
        function toggleFAQ(number) {
            const content = document.getElementById(`faq-content-${number}`);
            const icon = document.getElementById(`faq-icon-${number}`);
            
            content.classList.toggle('open');
            icon.classList.toggle('rotate-180');
        }
        // Open email client
        function openEmail() {
            document.getElementById('contactModal').style.display = "block";
        }
        // Open call popup and dialer
        function openCallPopup() {
            document.getElementById('call-modal').style.display = "block";
            window.location.href = "tel:667-355-2334";
        }
        // Open Privacy modal
        function openPrivacy() {
            document.getElementById('privacy-modal').style.display = "block";
        }
        // Open Terms modal
        function openTerms() {
            document.getElementById('terms-modal').style.display = "block";
        }
        // Close modals
        document.querySelectorAll('.close').forEach(closeBtn => {
            closeBtn.addEventListener('click', function() {
                this.parentElement.parentElement.style.display = "none";
            });
        });
        window.addEventListener('click', function(event) {
            if (event.target.classList.contains('modal')) {
                event.target.style.display = "none";
            }
        });
        // Form submission (placeholder)
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Form submitted! (This is a placeholder action)');
            document.getElementById('contactModal').style.display = 'none';
        });
    </script>
</body>
</html>
<!-- Policy and Procedures Modal -->
<div id="policy-modal" class="modal">
    <div class="modal-content" style="max-width: 90%; max-height: 90vh; overflow-y: auto;">
        <span class="close">&times;</span>
        <div id="policy-modal-content">
            <!-- The FULL Policy and Procedures form will be inserted here by JavaScript -->
        </div>
    </div>
</div>
<!-- Consent to Release Info Modal -->
<div id="consent-release-modal" class="modal">
    <div class="modal-content" style="max-width: 800px; max-height: 90vh; overflow-y: auto;">
        <span class="close">&times;</span>
        <div id="consent-release-content">
            <!-- The FULL Consent to Release form will be inserted here by JavaScript -->
        </div>
    </div>
</div>
<!-- Intake and Consent to Treat Modal -->
<div id="intake-modal" class="modal">
    <div class="modal-content" style="max-width: 90%; max-height: 90vh; overflow-y: auto;">
        <span class="close">&times;</span>
        <div id="intake-modal-content">
            <!-- The FULL Intake form will be inserted here by JavaScript -->
        </div>
    </div>
</div>
<!-- MDCHS Consent Forms Modal -->
<div id="mdchs-modal" class="modal">
    <div class="modal-content" style="max-width: 90%; max-height: 90vh; overflow-y: auto;">
        <span class="close">&times;</span>
        <div id="mdchs-modal-content">
            <!-- The FULL MDCHS forms will be inserted here by JavaScript -->
        </div>
    </div>
</div>
