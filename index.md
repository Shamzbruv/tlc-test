<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TLC Family Services - Growth Through Gentle Strength</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@500;600;700&family=Lato:wght@300;400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script src='https://cdn.jsdelivr.net/npm/fullcalendar@6.1.18/index.global.min.js'></script>
    <script src="https://apis.google.com/js/api.js"></script>
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
        .leaf-icon {
            width: 48px;
            height: 48px;
            background-color: #C7B8E3;
            -webkit-mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24'%3E%3Cpath d='M17 8C8 10 5.9 16.17 3.82 21.34l1.89.66.95-2.3c.48.17 1.02.3 1.59.36L8 24l2-2c2 3 6 3 8 3 6 0 10-5 10-11C20 3 12 3 2 5v3c8-2 10 5.6 10 9 0 2-1 4-3 4-2 0-3-1-3-2 0-2 4-5 8-5z'/%3E%3C/svg%3E");
            mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24'%3E%3Cpath d='M17 8C8 10 5.9 16.17 3.82 21.34l1.89.66.95-2.3c.48.17 1.02.3 1.59.36L8 24l2-2c2 3 6 3 8 3 6 0 10-5 10-11C20 3 12 3 2 5v3c8-2 10 5.6 10 9 0 2-1 4-3 4-2 0-3-1-3-2 0-2 4-5 8-5z'/%3E%3C/svg%3E");
        }
        .branches-icon {
            width: 48px;
            height: 48px;
            background-color: #C7B8E3;
            -webkit-mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24'%3E%3Cpath d='M19 17.3V18h-4v-3h-2v3H5v-4h3l-2.5-2.5 1.42-1.42L10 14.18l3.08-3.1 1.42 1.42L12 15h3v2.3M19 7V8h-4v3h-2V8H5v4h3l-2.5 2.5 1.42 1.42L10 9.82l3.08 3.1 1.42-1.42L12 8h3V7h4z'/%3E%3C/svg%3E");
            mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24'%3E%3Cpath d='M19 17.3V18h-4v-3h-2v3H5v-4h3l-2.5-2.5 1.42-1.42L10 14.18l3.08-3.1 1.42 1.42L12 15h3v2.3M19 7V8h-4v3h-2V8H5v4h3l-2.5 2.5 1.42 1.42L10 9.82l3.08 3.1 1.42-1.42L12 8h3V7h4z'/%3E%3C/svg%3E");
        }
        .phoenix-icon {
            width: 48px;
            height: 48px;
            background-color: #C7B8E3;
            -webkit-mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24'%3E%3Cpath d='M12 2c2.5 0 3.9 2.1 3.9 5.1 0 1.9-.8 3.2-2 5.1 2.2.3 4 2.3 4 4.6 0 2.6-2.1 4.2-5.9 4.2s-5.9-1.6-5.9-4.2c0-2.3 1.8-4.3 4-4.6-1.2-1.4-2-3.2-2-5.1C8.1 4.1 9.5 2 12 2m0 2c-.6 0-1.9.9-1.9 3.1 0 1.4.6 2.8 1.5 3.8l.4.5-.5.2c-1.7.5-3 2.1-3 3.5 0 1.5 1.3 2.2 3.9 2.2 2.6 0 3.9-.7 3.9-2.2 0-1.4-1.3-3-3-3.5l-.5-.2.4-.5c.9-1 1.5-2.4 1.5-3.8C13.9 4.9 12.6 4 12 4z'/%3E%3C/svg%3E");
            mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24'%3E%3Cpath d='M12 2c2.5 0 3.9 2.1 3.9 5.1 0 1.9-.8 3.2-2 5.1 2.2.3 4 2.3 4 4.6 0 2.6-2.1 4.2-5.9 4.2s-5.9-1.6-5.9-4.2c0-2.3 1.8-4.3 4-4.6-1.2-1.4-2-3.2-2-5.1C8.1 4.1 9.5 2 12 2m0 2c-.6 0-1.9.9-1.9 3.1 0 1.4.6 2.8 1.5 3.8l.4.5-.5.2c-1.7.5-3 2.1-3 3.5 0 1.5 1.3 2.2 3.9 2.2 2.6 0 3.9-.7 3.9-2.2 0-1.4-1.3-3-3-3.5l-.5-.2.4-.5c.9-1 1.5-2.4 1.5-3.8C13.9 4.9 12.6 4 12 4z'/%3E%3C/svg%3E");
        }
        .bg-watercolor {
            background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='100%25' height='100%25' viewBox='0 0 800 800'%3E%3Cg %3E%3Ccircle fill='%23C7B8E3' cx='400' cy='400' r='600'/%3E%3Ccircle fill='%23B0C4DE' cx='400' cy='400' r='500'/%3E%3Ccircle fill='%23C7B8E3' cx='400' cy='400' r='400'/%3E%3Ccircle fill='%23FFB6C1' cx='400' cy='400' r='300'/%3E%3Ccircle fill='%23B0C4DE' cx='400' cy='400' r='200'/%3E%3Ccircle fill='%23C7B8E3' cx='400' cy='400' r='100'/%3E%3C/g%3E%3C/svg%3E");
            background-attachment: fixed;
            background-size: cover;
            background-position: center;
            opacity: 0.1;
        }
        .accordion-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease;
        }
        .accordion-content.open {
            max-height: 1000px;
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
        #mc_embed_signup .mc-field-group {
            margin-bottom: 1rem;
        }
        #mc_embed_signup .indicates-required {
            display: none;
        }
        #mc_embed_signup .clear {
            text-align: center;
        }
        #mc_embed_signup .optionalParent > .clear {
            margin-top: 1rem;
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
                    <a href="#home" class="px-3 py-2 text-sm font-medium text-purple-900 border-b-2 border-transparent hover:border-purple-500">Home</a>
                    <a href="#services" class="px-3 py-2 text-sm font-medium text-purple-900 border-b-2 border-transparent hover:border-purple-500">Services</a>
                    <a href="#resources" class="px-3 py-2 text-sm font-medium text-purple-900 border-b-2 border-transparent hover:border-purple-500">Resources</a>
                    <a href="#events" class="px-3 py-2 text-sm font-medium text-purple-900 border-b-2 border-transparent hover:border-purple-500">Events</a>
                    <a href="#about" class="px-3 py-2 text-sm font-medium text-purple-900 border-b-2 border-transparent hover:border-purple-500">About Us</a>
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
                <a href="#home" class="text-purple-900 hover:text-purple-700 block px-3 py-2 rounded-md text-base font-medium">Home</a>
                <a href="#services" class="text-purple-900 hover:text-purple-700 block px-3 py-2 rounded-md text-base font-medium">Services</a>
                <a href="#resources" class="text-purple-900 hover:text-purple-700 block px-3 py-2 rounded-md text-base font-medium">Resources</a>
                <a href="#events" class="text-purple-900 hover:text-purple-700 block px-3 py-2 rounded-md text-base font-medium">Events</a>
                <a href="#about" class="text-purple-900 hover:text-purple-700 block px-3 py-2 rounded-md text-base font-medium">About Us</a>
                <a href="#" onclick="openEmail()" class="bg-purple-600 hover:bg-purple-700 text-white block px-3 py-2 rounded-md text-base font-medium transition duration-300">Contact Us</a>
            </div>
        </div>
    </nav>
    <!-- Hero Section with your local image -->
<section id="home" class="relative bg-blue-50 overflow-hidden">
    <div class="absolute inset-0 bg-watercolor"></div>
    <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-20 md:py-32">
        <div class="lg:grid lg:grid-cols-2 lg:gap-8 items-center">
            <div class="mb-12 lg:mb-0 text-center lg:text-left">
                <h1 class="font-serif text-4xl md:text-5xl font-bold text-purple-800 mb-6 leading-tight">Healing Starts Here – Virtual Therapy for All Ages</h1>
                <p class="text-xl text-pink-700 mb-8">Accepting help is the first step. We'll walk the rest with you.</p>
                <a href="#services" class="inline-block bg-purple-600 text-white font-medium px-8 py-3 rounded-lg hover:bg-purple-700 transition duration-300 shadow-lg">Explore Our Services</a>
            </div>
            <div class="flex justify-center">
                <!-- Replaced with new image -->
                <img src='https://i.postimg.cc/ncrCsgHY/tlc-logo.png' alt='TLC Family Services Logo' class="w-full max-w-md h-auto rounded-lg shadow-2xl object-contain">
            </div>
        </div>
    </div>
    <div class="wavy-divider h-16 -mt-8"></div>
</section>
    <!-- Services Section -->
    <section id="services" class="py-16 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="font-serif text-3xl font-bold text-purple-800 mb-4">Our Therapeutic Services</h2>
                <div class="w-24 h-1 bg-purple-500 mx-auto"></div>
            </div>
          
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <!-- Individual Therapy -->
                <div class="bg-purple-50 rounded-lg p-8 text-center hover:shadow-lg transition duration-300">
                    <div class="leaf-icon mx-auto mb-6"></div>
                    <h3 class="font-serif text-xl font-bold text-purple-800 mb-4">Individual Therapy</h3>
                    <p class="text-pink-700 mb-6">
                        Personalized one-on-one sessions for ages 5-60 to address anxiety, depression, and life transitions.
                    </p>
                    <a href="individual-therapy.html" class="text-purple-600 hover:text-purple-800 font-medium flex items-center justify-center">
                        Learn more <i class="fas fa-arrow-right ml-2"></i>
                    </a>
                </div>
              
                <!-- Family Therapy -->
                <div class="bg-purple-50 rounded-lg p-8 text-center hover:shadow-lg transition duration-300">
                    <div class="branches-icon mx-auto mb-6"></div>
                    <h3 class="font-serif text-xl font-bold text-purple-800 mb-4">Family Therapy</h3>
                    <p class="text-pink-700 mb-6">
                        Strengthen family bonds and improve communication with our expert-guided sessions.
                    </p>
                    <a href="family-therapy.html" class="text-purple-600 hover:text-purple-800 font-medium flex items-center justify-center">
                        Learn more <i class="fas fa-arrow-right ml-2"></i>
                    </a>
                </div>
              
                <!-- PRP Services -->
                <div class="bg-purple-50 rounded-lg p-8 text-center hover:shadow-lg transition duration-300">
                    <div class="phoenix-icon mx-auto mb-6"></div>
                    <h3 class="font-serif text-xl font-bold text-purple-800 mb-4">PRP Services</h3>
                    <p class="text-pink-700 mb-6">
                        Psychiatric Rehabilitation Program to help individuals develop skills for community living.
                    </p>
                    <a href="prp-services.html" class="text-purple-600 hover:text-purple-800 font-medium flex items-center justify-center">
                        Learn more <i class="fas fa-arrow-right ml-2"></i>
                    </a>
                </div>
              
                <!-- Substance Abuse Support -->
                <div class="bg-purple-50 rounded-lg p-8 text-center hover:shadow-lg transition duration-300">
                    <div class="phoenix-icon mx-auto mb-6"></div>
                    <h3 class="font-serif text-xl font-bold text-purple-800 mb-4">Substance Abuse Support</h3>
                    <p class="text-pink-700 mb-6">
                        Recovery is a journey. We provide the map with compassionate, evidence-based care.
                    </p>
                    <a href="substance-abuse-support.html" class="text-purple-600 hover:text-purple-800 font-medium flex items-center justify-center">
                        Learn more <i class="fas fa-arrow-right ml-2"></i>
                    </a>
                </div>
            </div>
        </div>
    </section>
    <!-- Approach Section -->
    <section class="py-16 bg-purple-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="lg:grid lg:grid-cols-2 lg:gap-16 items-center">
                <div class="mb-12 lg:mb-0">
                    <img src="https://i.postimg.cc/Wz570w2y/Chat-GPT-Image-Aug-9-2025-02-19-00-PM.png" alt="Our Approach" class="rounded-lg shadow-xl w-full">
                </div>
                <div>
                    <h2 class="font-serif text-3xl font-bold text-purple-800 mb-6">Our Approach</h2>
                    <p class="text-pink-700 mb-6">
                        At TLC Family Services, we believe in "Growth Through Gentle Strength." Our therapeutic approach combines evidence-based practices with compassionate care, creating a safe space for healing and personal development.
                    </p>
                    <div class="space-y-6">
                        <div class="flex">
                            <div class="flex-shrink-0">
                                <div class="flex items-center justify-center h-12 w-12 rounded-md bg-purple-600 text-white">
                                    <i class="fas fa-check"></i>
                                </div>
                            </div>
                            <div class="ml-4">
                                <h3 class="font-serif text-lg font-medium text-purple-800">Client-Centered</h3>
                                <p class="text-pink-700">
                                    Your unique needs and goals guide our therapeutic process.
                                </p>
                            </div>
                        </div>
                        <div class="flex">
                            <div class="flex-shrink-0">
                                <div class="flex items-center justify-center h-12 w-12 rounded-md bg-purple-600 text-white">
                                    <i class="fas fa-check"></i>
                                </div>
                            </div>
                            <div class="ml-4">
                                <h3 class="font-serif text-lg font-medium text-purple-800">Holistic</h3>
                                <p class="text-pink-700">
                                    We address mind, body, and spirit for comprehensive healing.
                                </p>
                            </div>
                        </div>
                        <div class="flex">
                            <div class="flex-shrink-0">
                                <div class="flex items-center justify-center h-12 w-12 rounded-md bg-purple-600 text-white">
                                    <i class="fas fa-check"></i>
                                </div>
                            </div>
                            <div class="ml-4">
                                <h3 class="font-serif text-lg font-medium text-purple-800">Strength-Based</h3>
                                <p class="text-pink-700">
                                    Building on your existing strengths to foster resilience.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- Upcoming Events -->
    <section id="events" class="py-16 bg-gray-100">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12">
                <h2 class="font-serif text-3xl font-bold text-purple-800 mb-4">Community Workshops & Group Sessions</h2>
                <div class="w-24 h-1 bg-purple-500 mx-auto"></div>
            </div>
            <div class="text-center mb-6">
                <button id="event-signup-btn" class="bg-purple-600 text-white px-6 py-2 rounded-lg hover:bg-purple-700 transition duration-300">Stay in the Loop</button>
                <p class="text-sm text-pink-700 mt-2">Sign up for notifications on new events</p>
            </div>
            <div class="bg-white rounded-lg shadow-md p-6 mb-12">
                <div id="calendar"></div>
            </div>
          
            <div id="event-cards" class="flex flex-wrap justify-center gap-8">
                <!-- Dynamic cards will be added here -->
            </div>
          
            <!-- Registration Modal Popup -->
            <div id="registration-modal" class="modal">
                <div class="modal-content">
                    <span class="close">&times;</span>
                    <h3 id="modal-event-title" class="font-serif text-2xl font-bold text-purple-800 mb-6">Register for Event</h3>
                    <form id="registration-form" class="space-y-4">
                        <input type="hidden" id="reg-event-name" name="event_name">
                        <div>
                            <label for="reg-name" class="block text-sm font-medium text-pink-700 mb-1">Full Name</label>
                            <input type="text" id="reg-name" name="name" required class="w-full px-4 py-2 border border-purple-300 rounded-lg">
                        </div>
                        <div>
                            <label for="reg-email" class="block text-sm font-medium text-pink-700 mb-1">Email</label>
                            <input type="email" id="reg-email" name="email" required class="w-full px-4 py-2 border border-purple-300 rounded-lg">
                        </div>
                        <div>
                            <label for="reg-phone" class="block text-sm font-medium text-pink-700 mb-1">Phone (Optional)</label>
                            <input type="tel" id="reg-phone" name="phone" class="w-full px-4 py-2 border border-purple-300 rounded-lg">
                        </div>
                        <button type="submit" class="w-full bg-purple-600 hover:bg-purple-700 text-white font-medium py-3 px-4 rounded-lg transition duration-300">Submit Registration</button>
                    </form>
                    <p id="registration-status" class="mt-2 text-center text-pink-600"></p>
                    <button id="add-to-calendar-btn" class="w-full mt-4 bg-pink-500 hover:bg-pink-600 text-white font-medium py-3 px-4 rounded-lg transition duration-300">Add to My Calendar</button>
                </div>
            </div>
            <!-- Privacy Policy Modal -->
            <div id="privacy-modal" class="modal">
                <div class="modal-content">
                    <span class="close">&times;</span>
                    <h3 class="font-serif text-2xl font-bold text-purple-800 mb-6">Privacy Policy</h3>
                    <p class="text-pink-700">
                        At TLC Family Services, your privacy is our priority. In compliance with U.S. health laws like HIPAA, we safeguard your personal health information (PHI) with encrypted storage and secure communications. We only share data with your consent for treatment, payment, or operations. You have rights to access, amend, or restrict your information. We never sell data and use it only for care delivery. For full details, contact us. This policy ensures trust in your healing journey.
                    </p>
                </div>
            </div>
            <!-- Terms of Service Modal -->
            <div id="terms-modal" class="modal">
                <div class="modal-content">
                    <span class="close">&times;</span>
                    <h3 class="font-serif text-2xl font-bold text-purple-800 mb-6">Terms of Service</h3>
                    <p class="text-pink-700">
                        By using TLC Family Services, you agree to our terms. We provide virtual therapy in compliance with U.S. health regulations, including confidentiality under HIPAA. Services are for informational and therapeutic purposes; not for emergencies (call 911 or 988). Payment terms: Sessions are billed per agreement; cancellations require 24-hour notice or fees apply. We reserve the right to terminate services if guidelines aren't followed. Your participation is voluntary, and we're committed to ethical care. Contact us for questions.
                    </p>
                </div>
            </div>
            <!-- Event Signup Modal -->
            <div id="event-signup-modal" class="modal">
                <div class="modal-content">
                    <span class="close">&times;</span>
                    <h3 class="font-serif text-2xl font-bold text-purple-800 mb-6">Sign Up for Event Notifications</h3>
                    <p class="text-pink-700 mb-4">Enter your details below to receive emails whenever we add new events or workshops.</p>
                    <div id="mc_embed_shell">
<div id="mc_embed_signup">
    <form action="https://tlcfamilyservices.us19.list-manage.com/subscribe/post?u=005430ac176f7ff244f286e92&amp;id=7ac99b39ae&amp;f_id=00f7c2e1f0" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate space-y-4" target="_self" novalidate="">
        <div id="mc_embed_signup_scroll">
            <div class="mc-field-group"><label class="block text-sm font-medium text-pink-700 mb-1" for="mce-EMAIL">Email Address <span class="asterisk">*</span></label><input type="email" name="EMAIL" class="required email w-full px-4 py-2 border border-purple-300 rounded-lg focus:ring-purple-500 focus:border-purple-500" id="mce-EMAIL" required="" value=""></div><div class="mc-field-group"><label class="block text-sm font-medium text-pink-700 mb-1" for="mce-FNAME">Full Name </label><input type="text" name="FNAME" class=" text w-full px-4 py-2 border border-purple-300 rounded-lg focus:ring-purple-500 focus:border-purple-500" id="mce-FNAME" value=""></div>
        <div id="mce-responses" class="clear foot">
            <div class="response" id="mce-error-response" style="display: none;"></div>
            <div class="response" id="mce-success-response" style="display: none;"></div>
        </div>
    <div aria-hidden="true" style="position: absolute; left: -5000px;">
        /* real people should not fill this in and expect good things - do not remove this or risk form bot signups */
        <input type="text" name="b_005430ac176f7ff244f286e92_7ac99b39ae" tabindex="-1" value="">
    </div>
        <div class="optionalParent">
            <div class="clear foot">
                <input type="submit" name="subscribe" id="mc-embedded-subscribe" class="w-full bg-purple-600 hover:bg-purple-700 text-white font-medium py-3 px-4 rounded-lg transition duration-300" value="Subscribe">
            </div>
        </div>
    </div>
</form>
</div>
</div>
                    <p class="text-xs text-pink-700 mt-4">We'll email you about new events. Unsubscribe anytime.</p>
                </div>
            </div>
        </div>
    </section>
    <!-- Client Resources Hub -->
    <section id="resources" class="py-16 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12">
                <h2 class="font-serif text-3xl font-bold text-purple-800 mb-4">Client Resources</h2>
                <div class="w-24 h-1 bg-purple-500 mx-auto"></div>
            </div>
          
            <!-- New Client Onboarding and Consent -->
            <div class="bg-purple-100 rounded-lg p-8 mb-12 border-2 border-purple-400">
                <div class="flex items-center mb-6">
                    <div class="w-14 h-14 rounded-full bg-purple-200 flex items-center justify-center mr-4">
                        <i class="fas fa-exclamation-circle text-purple-700 text-2xl"></i>
                    </div>
                    <h3 class="font-serif text-2xl font-bold text-purple-800">New Client Onboarding and Consent</h3>
                </div>
                <p class="text-pink-700 mb-6 font-semibold">This section is critical for all new clients. Please click each link below, open in a new tab, and read each document carefully to proceed with your therapy journey.</p>
                <div class="space-y-4">
                    <a href="consent-forms/policies-and-procedures.html" target="_blank" class="block bg-white text-purple-800 font-medium py-3 px-4 rounded-lg hover:bg-purple-50 transition duration-300 flex items-center justify-between">
                        <span>Policies and Procedures</span>
                        <span class="text-sm text-gray-600">(~15 min)</span>
                    </a>
                    <a href="consent-forms/consent-to-release.html" target="_blank" class="block bg-white text-purple-800 font-medium py-3 px-4 rounded-lg hover:bg-purple-50 transition duration-300 flex items-center justify-between">
                        <span>Consent to Release Information</span>
                        <span class="text-sm text-gray-600">(~5 min)</span>
                    </a>
                    <a href="consent-forms/intake-consent-to-treat.html" target="_blank" class="block bg-white text-purple-800 font-medium py-3 px-4 rounded-lg hover:bg-purple-50 transition duration-300 flex items-center justify-between">
                        <span>Intake and Consent to Treat</span>
                        <span class="text-sm text-gray-600">(~10 min)</span>
                    </a>
                    <a href="consent-forms/additional-consent-forms.html" target="_blank" class="block bg-white text-purple-800 font-medium py-3 px-4 rounded-lg hover:bg-purple-50 transition duration-300 flex items-center justify-between">
                        <span>Additional Consent Forms</span>
                        <span class="text-sm text-gray-600">(~20 min)</span>
                    </a>
                </div>
            </div>
          
            <!-- Request Information Form -->
            <div class="bg-purple-50 rounded-lg p-8 mb-12">
                <div class="flex items-center mb-6">
                    <div class="w-14 h-14 rounded-full bg-purple-100 flex items-center justify-center mr-4">
                        <i class="fas fa-question-circle text-purple-700 text-2xl"></i>
                    </div>
                    <h3 class="font-serif text-2xl font-bold text-purple-800">Request Information</h3>
                </div>
                <p class="text-pink-700 mb-6">Have questions? Our team is here to help. Fill out the form below and we'll respond within 24 hours.</p>
              
                <form id="request-form" action="https://formspree.io/f/mzzvjdow" method="POST" class="space-y-4">
                    <div>
                        <label for="name" class="block text-sm font-medium text-pink-700 mb-1">Full Name</label>
                        <input type="text" id="name" name="name" class="w-full px-4 py-2 border border-purple-300 rounded-lg focus:ring-purple-500 focus:border-purple-500">
                    </div>
                  
                    <div>
                        <label for="email" class="block text-sm font-medium text-pink-700 mb-1">Email Address</label>
                        <input type="email" id="email" name="email" class="w-full px-4 py-2 border border-purple-300 rounded-lg focus:ring-purple-500 focus:border-purple-500">
                    </div>
                  
                    <div>
                        <label for="phone" class="block text-sm font-medium text-pink-700 mb-1">Phone Number (Optional)</label>
                        <input type="tel" id="phone" name="phone" class="w-full px-4 py-2 border border-purple-300 rounded-lg focus:ring-purple-500 focus:border-purple-500">
                    </div>
                  
                    <div>
                        <label for="help-with" class="block text-sm font-medium text-pink-700 mb-1">I need help with:</label>
                        <select id="help-with" name="help-with" class="w-full px-4 py-2 border border-purple-300 rounded-lg focus:ring-purple-500 focus:border-purple-500">
                            <option value="">Select an option</option>
                            <option value="individual-therapy">Individual Therapy</option>
                            <option value="family-therapy">Family Therapy</option>
                            <option value="prp-services">PRP Services</option>
                            <option value="substance-abuse">Substance Abuse Support</option>
                            <option value="other">Other</option>
                        </select>
                    </div>
                  
                    <div>
                        <label for="message" class="block text-sm font-medium text-pink-700 mb-1">Your Question</label>
                        <textarea id="message" name="message" rows="4" class="w-full px-4 py-2 border border-purple-300 rounded-lg focus:ring-purple-500 focus:border-purple-500"></textarea>
                    </div>
                  
                    <button type="submit" class="w-full bg-purple-600 hover:bg-purple-700 text-white font-medium py-3 px-4 rounded-lg transition duration-300">Submit Request</button>
                </form>
                <p id="request-status" class="mt-2 text-center text-pink-600"></p>
            </div>
          
            <!-- Helpful Resources -->
            <div class="mt-16">
                <h3 class="font-serif text-3xl font-bold text-purple-800 mb-6 text-center">Helpful Resources</h3>
                <div class="grid md:grid-cols-3 gap-6">
                    <div class="bg-purple-50 rounded-lg p-6 hover:shadow-md transition duration-300">
                        <div class="flex items-center mb-4">
                            <i class="fas fa-file-pdf text-3xl text-purple-500 mr-4"></i>
                            <h4 class="font-serif text-lg font-medium text-purple-800">Signs Your Loved One Needs Help</h4>
                        </div>
                        <p class="text-pink-700 mb-4">A guide to recognizing when someone may be struggling with substance abuse or mental health issues.</p>
                        <a href="#" onclick="openSignsModal()" class="text-purple-600 hover:text-purple-800 font-medium">View Content <i class="fas fa-eye ml-2"></i></a>
                    </div>
                  
                    <div class="bg-purple-50 rounded-lg p-6 hover:shadow-md transition duration-300">
                        <div class="flex items-center mb-4">
                            <i class="fas fa-file-pdf text-3xl text-purple-500 mr-4"></i>
                            <h4 class="font-serif text-lg font-medium text-purple-800">Coping Skills Toolkit</h4>
                        </div>
                        <p class="text-pink-700 mb-4">Practical exercises and strategies for managing anxiety, depression, and stress.</p>
                        <a href="#" onclick="openCopingModal()" class="text-purple-600 hover:text-purple-800 font-medium">View Content <i class="fas fa-eye ml-2"></i></a>
                    </div>
                  
                    <div class="bg-purple-50 rounded-lg p-6 hover:shadow-md transition duration-300">
                        <div class="flex items-center mb-4">
                            <i class="fas fa-file-pdf text-3xl text-purple-500 mr-4"></i>
                            <h4 class="font-serif text-lg font-medium text-purple-800">Parenting Through Challenges</h4>
                        </div>
                        <p class="text-pink-700 mb-4">Tips for maintaining strong family connections during difficult times.</p>
                        <a href="#" onclick="openParentingModal()" class="text-purple-600 hover:text-purple-800 font-medium">View Content <i class="fas fa-eye ml-2"></i></a>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- About Us -->
    <section id="about" class="py-16 bg-purple-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="lg:grid lg:grid-cols-2 lg:gap-12 items-center">
                <div class="mb-12 lg:mb-0">
                    <h2 class="font-serif text-3xl font-bold text-purple-800 mb-6">About TLC Family Services</h2>
                    <p class="text-pink-700 mb-6">TLC Family Services has guided 500+ clients through life's toughest moments since 2021. Our virtual platform removes barriers to care.</p>
                    <p class="text-pink-700 mb-6">Founded by a team of experienced mental health professionals, we recognized the need for accessible, compassionate care that meets people where they are—literally and figuratively.</p>
                    <p class="text-pink-700 mb-8">Our evidence-based approaches combined with personalized attention create meaningful change for individuals and families across all age groups and backgrounds.</p>
                  
                    <div class="grid sm:grid-cols-2 gap-6">
                        <div class="bg-white p-6 rounded-lg shadow-sm">
                            <h3 class="font-serif text-xl font-bold text-purple-800 mb-3">Our Mission</h3>
                            <p class="text-pink-700">To provide exceptional, accessible mental health services that empower individuals and families to thrive.</p>
                        </div>
                        <div class="bg-white p-6 rounded-lg shadow-sm">
                            <h3 class="font-serif text-xl font-bold text-purple-800 mb-3">Our Vision</h3>
                            <p class="text-pink-700">A world where quality mental health care is available to all who need it, without stigma or barriers.</p>
                        </div>
                    </div>
                </div>
              
                <div class="relative">
                    <img src="https://i.postimg.cc/26FGSfgr/b634e4ae-2a89-4c8b-9f3e-0a3d42ccbdb3.jpg" alt="Our Team" class="rounded-lg shadow-xl w-full">
                    <div class="absolute -bottom-6 -right-6 bg-white p-6 rounded-lg shadow-lg w-3/4">
                        <h3 class="font-serif text-lg font-bold text-purple-800 mb-2">Our Team</h3>
                        <p class="text-pink-700">Licensed professionals with specialized training in trauma, family systems, and evidence-based interventions.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- Call to Action -->
    <section class="py-16 bg-purple-800 text-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="font-serif text-3xl font-bold mb-6">Ready to Begin Your Healing Journey?</h2>
            <p class="text-purple-100 max-w-2xl mx-auto mb-8">
                Take the first step toward growth and healing. Our compassionate team is here to support you.
            </p>
            <div class="flex flex-col sm:flex-row justify-center gap-4">
                <a href="#" onclick="openEmail()" class="px-8 py-3 rounded-lg bg-pink-500 hover:bg-pink-600 text-white font-medium transition duration-300 transform hover:scale-105">
                    Contact Us
                </a>
                <a href="#" onclick="openCallPopup()" class="px-8 py-3 rounded-lg border-2 border-white hover:bg-white hover:text-purple-800 font-medium transition duration-300"><i class="fas fa-phone mr-2"></i> Call Now</a>
            </div>
        </div>
    </section>
    <!-- Footer -->
    <footer class="bg-purple-900 text-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
            <div class="grid md:grid-cols-4 gap-8">
                <div>
                    <div class="flex items-center">
                        <img src='https://i.postimg.cc/ncrCsgHY/tlc-logo.png' alt='tlc-logo' class="h-8 w-8">
                        <span class="ml-2 font-serif text-xl font-bold text-purple-300">TLC Family Services</span>
                    </div>
                    <p class="mt-4 text-purple-300 text-sm">
                        Growth Through Gentle Strength
                    </p>
                </div>
              
                <div>
                    <h3 class="font-serif text-lg font-bold mb-4">Quick Links</h3>
                    <ul class="space-y-2">
                        <li><a href="#home" class="text-purple-300 hover:text-white text-sm">Home</a></li>
                        <li><a href="#services" class="text-purple-300 hover:text-white text-sm">Services</a></li>
                        <li><a href="#resources" class="text-purple-300 hover:text-white text-sm">Resources</a></li>
                        <li><a href="#events" class="text-purple-300 hover:text-white text-sm">Events</a></li>
                        <li><a href="#about" class="text-purple-300 hover:text-white text-sm">About Us</a></li>
                    </ul>
                </div>
              
                <div>
                    <h3 class="font-serif text-lg font-bold mb-4">Contact Us</h3>
                    <ul class="space-y-2 text-purple-300 text-sm">
                        <li>Tres Ladson</li>
                        <li><a href="#" onclick="openEmail()">Admin@tlcfamilyservices.com</a></li>
                        <li><a href="#" onclick="openCallPopup()">667-355-2334</a></li>
                        <li>Online-based services</li>
                    </ul>
                </div>
              
                <div>
                    <h3 class="font-serif text-lg font-bold mb-4">Follow Us</h3>
                    <div class="flex space-x-4">
                        <a href="https://www.instagram.com/tlc_familyservices?igsh=MTg5NTNva3lidGMxeg==" class="text-purple-300 hover:text-white">
                            <i class="fab fa-instagram text-xl"></i>
                        </a>
                    </div>
                  
                    <h3 class="font-serif text-lg font-bold mt-6 mb-3">Subscribe to Newsletter</h3>
                    <form class="flex">
                        <input type="email" placeholder="Your email" class="px-4 py-2 rounded-l-lg text-purple-900 w-full">
                        <button type="submit" class="bg-purple-600 hover:bg-purple-700 px-4 py-2 rounded-r-lg transition duration-300"><i class="fas fa-paper-plane text-white"></i></button>
                    </form>
                </div>
            </div>
          
            <div class="border-t border-purple-800 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-purple-300 text-sm mb-4 md:mb-0">© 2023 TLC Family Services. All rights reserved.</p>
                <div class="flex space-x-6">
                    <a href="#" onclick="openPrivacy()" class="text-purple-300 hover:text-white text-sm">Privacy Policy</a>
                    <a href="#" onclick="openTerms()" class="text-purple-300 hover:text-white text-sm">Terms of Service</a>
                    <a href="#" class="text-purple-300 hover:text-white text-sm">HIPAA Compliance</a>
                </div>
            </div>
          
            <div class="mt-4 text-center md:text-left">
                <p class="text-purple-400 text-xs italic">TLC Family Services does not provide emergency care. If you're in crisis, call 988 or go to your nearest emergency room.</p>
            </div>
        </div>
    </footer>
    <!-- Call Popup Modal -->
    <div id="call-modal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <h3 class="font-serif text-2xl font-bold text-purple-800 mb-6">Call Us</h3>
            <p class="text-pink-700 text-center">667-355-2334</p>
        </div>
    </div>
    <!-- Signs Modal -->
    <div id="signs-modal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <h2 class="font-serif text-2xl font-bold text-purple-800 mb-6">Signs Your Loved One Needs Help (Substance Abuse/Mental Health Guide)</h2>
            <h3 class="font-serif text-xl text-purple-800 mb-2">Recognizing the Signs</h3>
            <ul class="list-disc list-inside text-pink-700 mb-4">
                <li>Behavioral Changes: Withdrawal from social activities, sudden mood swings, or neglect of responsibilities.</li>
                <li>Physical Signs: Unexplained weight loss, poor hygiene, or frequent illness.</li>
                <li>Emotional Clues: Increased irritability, hopelessness, or expressions of guilt/shame.</li>
            </ul>
            <h3 class="font-serif text-xl text-purple-800 mb-2">How to Approach Them</h3>
            <ul class="list-disc list-inside text-pink-700 mb-4">
                <li>Do: Use "I" statements ("I've noticed you seem stressed—I'm here to listen.").</li>
                <li>Avoid: Blame or ultimatums ("You're ruining your life!").</li>
            </ul>
            <h3 class="font-serif text-xl text-purple-800 mb-2">Next Steps</h3>
            <ul class="list-disc list-inside text-pink-700 mb-4">
                <li>Offer to help research therapists or support groups together.</li>
                <li>Crisis Resources: Include hotlines (e.g., SAMHSA: 1-800-662-HELP).</li>
            </ul>
            <p class="text-pink-700 italic">Your support matters. Small actions can be the first step toward their recovery.</p>
        </div>
    </div>
    <!-- Coping Modal -->
    <div id="coping-modal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <h2 class="font-serif text-2xl font-bold text-purple-800 mb-6">Coping Skills Toolkit (Anxiety/Depression/Stress Management)</h2>
            <h3 class="font-serif text-xl text-purple-800 mb-2">Quick Grounding Techniques</h3>
            <ul class="list-disc list-inside text-pink-700 mb-4">
                <li>5-4-3-2-1 Method: Name 5 things you see, 4 you feel, 3 you hear, 2 you smell, 1 you taste.</li>
                <li>Breathing Exercise: Box breathing (inhale 4 sec, hold 4 sec, exhale 4 sec).</li>
            </ul>
            <h3 class="font-serif text-xl text-purple-800 mb-2">Daily Practices</h3>
            <ul class="list-disc list-inside text-pink-700 mb-4">
                <li>Gratitude Journal: Write 3 things you're thankful for each morning.</li>
                <li>Movement: A 10-minute walk to reset your mood.</li>
            </ul>
            <h3 class="font-serif text-xl text-purple-800 mb-2">When Overwhelmed</h3>
            <ul class="list-disc list-inside text-pink-700 mb-4">
                <li>Self-Compassion Reminder: "This feeling is temporary. I've gotten through hard times before."</li>
                <li>Distraction Ideas: Call a friend, organize a drawer, or listen to upbeat music.</li>
            </ul>
            <p class="text-pink-700 italic">Healing isn't linear. Celebrate small wins—they add up.</p>
        </div>
    </div>
    <!-- Parenting Modal -->
    <div id="parenting-modal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <h2 class="font-serif text-2xl font-bold text-purple-800 mb-6">Parenting Through Challenges (Family Connection Tips)</h2>
            <h3 class="font-serif text-xl text-purple-800 mb-2">Staying Connected</h3>
            <ul class="list-disc list-inside text-pink-700 mb-4">
                <li>Rituals Matter: Weekly game nights or shared meals (even 15 minutes counts).</li>
                <li>Active Listening: Reflect their feelings ("It sounds like you're frustrated about school.").</li>
            </ul>
            <h3 class="font-serif text-xl text-purple-800 mb-2">Navigating Conflict</h3>
            <ul class="list-disc list-inside text-pink-700 mb-4">
                <li>Use "We" Language: "How can we solve this together?"</li>
                <li>Time-Ins: Pause heated moments with a walk or quiet activity.</li>
            </ul>
            <h3 class="font-serif text-xl text-purple-800 mb-2">Self-Care for Parents</h3>
            <ul class="list-disc list-inside text-pink-700 mb-4">
                <li>Micro-Breaks: Deep breaths while making coffee, or a 5-minute stretch.</li>
                <li>Ask for Help: Swap childcare with a friend or join a parent support group.</li>
            </ul>
            <p class="text-pink-700 italic">You don't have to be perfect. Showing up consistently is enough.</p>
        </div>
    </div>
    <script>
        // Mobile menu toggle
        document.getElementById('mobile-menu-button').addEventListener('click', function() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        });
        // Open email client
        function openEmail() {
            window.location.href = "mailto:Admin@tlcfamilyservices.com";
        }
        // Open call popup and dialer
        function openCallPopup() {
            document.getElementById('call-modal').style.display = "block";
            window.location.href = "tel:667-355-2334";
        }
        // Open Signs Modal
        function openSignsModal() {
            document.getElementById('signs-modal').style.display = "block";
        }
        // Open Coping Modal
        function openCopingModal() {
            document.getElementById('coping-modal').style.display = "block";
        }
        // Open Parenting Modal
        function openParentingModal() {
            document.getElementById('parenting-modal').style.display = "block";
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
        // Async submission for request form (with status)
        document.getElementById('request-form').addEventListener('submit', async function(e) {
            e.preventDefault();
            const status = document.getElementById('request-status');
            const data = new FormData(e.target);
            fetch(e.target.action, {
                method: 'POST',
                body: data,
                headers: {
                    'Accept': 'application/json'
                }
            }).then(response => {
                if (response.ok) {
                    status.innerHTML = "Thanks for your submission!";
                    e.target.reset();
                } else {
                    response.json().then(data => {
                        status.innerHTML = data.errors ? data.errors.map(error => error.message).join(", ") : "Oops! Problem submitting form.";
                    });
                }
            }).catch(error => {
                status.innerHTML = "Oops! Problem submitting form.";
            });
        });
        // Async submission for registration form (in modal, with status)
        document.getElementById('registration-form').addEventListener('submit', async function(e) {
            e.preventDefault();
            const status = document.getElementById('registration-status');
            const data = new FormData(e.target);
            fetch(e.target.action, {
                method: 'POST',
                body: data,
                headers: {
                    'Accept': 'application/json'
                }
            }).then(response => {
                if (response.ok) {
                    status.innerHTML = "Thanks for your submission!";
                    e.target.reset();
                } else {
                    response.json().then(data => {
                        status.innerHTML = data.errors ? data.errors.map(error => error.message).join(", ") : "Oops! Problem submitting form.";
                    });
                }
            }).catch(error => {
                status.innerHTML = "Oops! Problem submitting form.";
            });
        });
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
              
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    targetElement.scrollIntoView({
                        behavior: 'smooth'
                    });
                }
            });
        });
        // Calendar initialization - fetches from Google
        document.addEventListener('DOMContentLoaded', function() {
            var calendarEl = document.getElementById('calendar');
            calendar = new FullCalendar.Calendar(calendarEl, {
              initialView: 'dayGridMonth',
              events: function(fetchInfo, successCallback, failureCallback) {
                fetch(`https://www.googleapis.com/calendar/v3/calendars/admin%40tlcfamilyservices.com/events?key=AIzaSyBo41-vJOgIizG6SC8nRH85-jjrlV7f4vw&timeMin=${fetchInfo.start.toISOString()}&timeMax=${fetchInfo.end.toISOString()}&singleEvents=true&orderBy=startTime`)
                  .then(response => response.json())
                  .then(data => {
                    if (data.error) {
                      console.error('Error fetching events:', data.error);
                      successCallback([]);
                      generateEventCards([]);
                      return;
                    }
                    let events = data.items.map(event => ({
                        id: event.id,
                        title: event.summary,
                        start: event.start.dateTime || event.start.date,
                        end: event.end.dateTime || event.end.date,
                        description: event.description || 'No description'
                    }));
                    successCallback(events);
                    generateEventCards(events);
                  })
                  .catch(error => {
                    console.error('Error fetching events:', error);
                    successCallback([]);
                    generateEventCards([]);
                  });
              }
            });
            calendar.render();
            // Auto-refresh every 30 seconds
            setInterval(function() {
                calendar.refetchEvents();
            }, 30000);
            // Add to Calendar Button in Modal
            document.getElementById('add-to-calendar-btn').addEventListener('click', function() {
                downloadICS();
            });
            // Close Modal
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
        });
        function generateEventCards(events) {
            const container = document.getElementById('event-cards');
            container.innerHTML = ''; // Clear existing cards
            const upcomingEvents = events
                .filter(event => new Date(event.start) > new Date()) // Upcoming only
                .sort((a, b) => new Date(a.start) - new Date(b.start)) // Sort by date
                .slice(0, 3); // Max 3
            if (upcomingEvents.length === 0) {
                container.innerHTML = '<p class="text-center text-pink-700 col-span-full">No upcoming events</p>';
                return;
            }
            // Center based on count
            let colsClass = 'grid-cols-3';
            if (upcomingEvents.length === 1) {
                colsClass = 'grid-cols-1';
            } else if (upcomingEvents.length === 2) {
                colsClass = 'grid-cols-2';
            }
            container.classList.add('grid', colsClass, 'gap-8', 'justify-center');
            upcomingEvents.forEach(event => {
                const date = new Date(event.start);
                const month = date.toLocaleString('default', { month: 'short' }).toUpperCase();
                const day = date.getDate();
                const time = date.toLocaleTimeString([], {hour: 'numeric', minute: '2-digit', timeZoneName: 'short'}).replace(' GMT-5', ' EST'); // Adjust timezone as needed
                const card = document.createElement('div');
                card.className = 'bg-purple-50 rounded-lg p-8 max-w-xs';
                card.innerHTML = `
                    <div class="flex items-center mb-4">
                        <div class="bg-purple-100 text-purple-800 rounded-lg px-4 py-2 mr-4">
                            <div class="text-2xl font-bold">${day}</div>
                            <div class="text-sm uppercase">${month}</div>
                        </div>
                        <div>
                            <h3 class="font-serif text-lg font-bold text-purple-800">${event.title}</h3>
                            <p class="text-pink-700">${time}</p>
                        </div>
                    </div>
                    <p class="text-pink-700 mb-4">${event.description}</p>
                    <a href="#" class="register-btn text-purple-600 font-medium hover:text-purple-800" data-event-id="${event.id}" data-event-title="${event.title}" data-event-start="${event.start}" data-event-end="${event.end}" data-event-desc="${event.description}">Register Now <i class="fas fa-arrow-right ml-1"></i></a>
                `;
                container.appendChild(card);
            });
            // Add click listeners to register buttons
            document.querySelectorAll('.register-btn').forEach(btn => {
                btn.addEventListener('click', function(e) {
                    e.preventDefault();
                    const modal = document.getElementById('registration-modal');
                    document.getElementById('modal-event-title').textContent = `Register for ${this.dataset.eventTitle}`;
                    document.getElementById('reg-event-name').value = this.dataset.eventTitle;
                    currentEvent = {
                        title: this.dataset.eventTitle,
                        start: this.dataset.eventStart,
                        end: this.dataset.eventEnd || this.dataset.eventStart, // Use start if no end
                        description: this.dataset.eventDesc
                    };
                    modal.style.display = "block";
                });
            });
        }
        let currentEvent = {}; // To store event for .ics
        function closeModal() {
            document.getElementById('registration-modal').style.display = "none";
        }
        function downloadICS() {
            const icsContent = `BEGIN:VCALENDAR
VERSION:2.0
BEGIN:VEVENT
SUMMARY:${currentEvent.title}
DTSTART:${new Date(currentEvent.start).toUTCString().replace(/ GMT/, 'Z')}
DTEND:${new Date(currentEvent.end).toUTCString().replace(/ GMT/, 'Z')}
DESCRIPTION:${currentEvent.description}
END:VEVENT
END:VCALENDAR`;
            const blob = new Blob([icsContent], { type: 'text/calendar' });
            const url = URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = `${currentEvent.title}.ics`;
            document.body.appendChild(a);
            a.click();
            document.body.removeChild(a);
            URL.revokeObjectURL(url);
            closeModal();
        }
        // Open event signup modal
        document.getElementById('event-signup-btn').addEventListener('click', function() {
            document.getElementById('event-signup-modal').style.display = "block";
        });
    </script>
</body>
</html>
