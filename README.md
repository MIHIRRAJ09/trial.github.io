<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mihir's Professional Portfolio</title>
    <!-- Load Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Configure Tailwind for Inter font and custom colors -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'exl-blue': '#1e3a8a', // A deep blue color
                        'fms-gold': '#d97706', // A rich orange/gold
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    <style>
        /* Ensuring smooth scroll behavior for navigation */
        html {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="font-sans bg-gray-50 text-gray-800">

    <!-- Navbar (Fixed and Responsive) -->
    <header class="sticky top-0 z-50 bg-white shadow-lg">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <!-- Logo/Name -->
                <a href="#" class="text-xl font-extrabold text-exl-blue tracking-wide">Mihir.Dev</a>

                <!-- Desktop Navigation Links -->
                <nav class="hidden md:flex space-x-8">
                    <a href="#home" class="text-gray-600 hover:text-exl-blue transition duration-300 font-medium">Home</a>
                    <a href="#skills" class="text-gray-600 hover:text-exl-blue transition duration-300 font-medium">Skills</a>
                    <a href="#goals" class="text-gray-600 hover:text-exl-blue transition duration-300 font-medium">Goals</a>
                    <a href="#contact" class="text-gray-600 hover:text-exl-blue transition duration-300 font-medium">Contact</a>
                </nav>

                <!-- Mobile Menu Button (Toggle via JS) -->
                <button id="mobile-menu-button" class="md:hidden p-2 text-gray-500 hover:text-exl-blue focus:outline-none">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path></svg>
                </button>
            </div>
        </div>

        <!-- Mobile Menu (Hidden by default) -->
        <div id="mobile-menu" class="hidden md:hidden bg-white shadow-md border-t border-gray-100">
            <nav class="px-2 pt-2 pb-3 space-y-1 sm:px-3 flex flex-col">
                <a href="#home" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:bg-gray-100" onclick="closeMobileMenu()">Home</a>
                <a href="#skills" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:bg-gray-100" onclick="closeMobileMenu()">Skills</a>
                <a href="#goals" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:bg-gray-100" onclick="closeMobileMenu()">Goals</a>
                <a href="#contact" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:bg-gray-100" onclick="closeMobileMenu()">Contact</a>
            </nav>
        </div>
    </header>

    <main>
        <!-- 1. Hero Section (Home) -->
        <section id="home" class="relative bg-white py-24 md:py-32 overflow-hidden border-b-4 border-fms-gold">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
                <div class="relative z-10">
                    <span class="text-lg font-semibold text-fms-gold uppercase tracking-widest">Consultant & Strategist</span>
                    <h1 class="mt-4 text-5xl md:text-7xl font-extrabold tracking-tight text-gray-900">
                        Mihir's <span class="text-exl-blue">Professional</span> Hub
                    </h1>
                    <p class="mt-6 text-xl text-gray-500 max-w-2xl mx-auto">
                        Leveraging IIT/FMS expertise in Data, Strategy, and Project Management to drive high-impact results at EXL for NBA. Focused on continuous personal and professional growth.
                    </p>
                    <div class="mt-10 flex justify-center space-x-4">
                        <a href="#skills" class="inline-flex items-center px-6 py-3 border border-transparent text-base font-medium rounded-xl shadow-lg text-white bg-exl-blue hover:bg-indigo-700 transition duration-300 transform hover:scale-105">
                            View Core Skills
                        </a>
                        <a href="#contact" class="inline-flex items-center px-6 py-3 border border-exl-blue text-base font-medium rounded-xl text-exl-blue bg-white hover:bg-exl-blue hover:text-white transition duration-300 transform hover:scale-105">
                            Connect Today
                        </a>
                    </div>
                </div>
            </div>
        </section>

        <!-- 2. Skills Section -->
        <section id="skills" class="py-20 bg-gray-100 border-b border-gray-200">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center">
                    <h2 class="text-3xl font-extrabold text-gray-900 sm:text-4xl">Core Professional Skills</h2>
                    <p class="mt-4 text-lg text-gray-500">
                        A blend of technical, analytical, and managerial expertise from leading institutions.
                    </p>
                </div>

                <div class="mt-12 grid grid-cols-1 gap-8 sm:grid-cols-2 lg:grid-cols-3">
                    <!-- Skill Card 1 -->
                    <div class="p-6 bg-white rounded-xl shadow-2xl transition duration-500 transform hover:shadow-exl-blue/30 hover:-translate-y-1">
                        <div class="flex items-center space-x-4">
                            <div class="flex-shrink-0 bg-exl-blue text-white rounded-full p-3">
                                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 19V6l12-3v13M9 19h12M9 19c0 1.105-1.791 2-4 2s-4-.895-4-2 1.791-2 4-2 4 .895 4 2zM12 6c0 1.105-1.791 2-4 2s-4-.895-4-2 1.791-2 4-2 4 .895 4 2zM12 18h8"></path></svg>
                            </div>
                            <h3 class="text-xl font-semibold text-gray-900">Data Analytics & BI</h3>
                        </div>
                        <p class="mt-4 text-gray-600">Expert in SQL for querying and Tableau for data visualization and business intelligence reporting.</p>
                        <ul class="mt-4 space-y-2 text-sm text-gray-500 list-disc list-inside">
                            <li>SQL Database Management</li>
                            <li>Tableau Dashboard Design</li>
                        </ul>
                    </div>

                    <!-- Skill Card 2 -->
                    <div class="p-6 bg-white rounded-xl shadow-2xl transition duration-500 transform hover:shadow-exl-blue/30 hover:-translate-y-1">
                        <div class="flex items-center space-x-4">
                            <div class="flex-shrink-0 bg-fms-gold text-white rounded-full p-3">
                                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11 5H6a2 2 0 00-2 2v11a2 2 0 002 2h11a2 2 0 002-2v-5m-1.414-9.414a2 2 0 112.828 2.828L11.828 15H9v-2.828l8.586-8.586z"></path></svg>
                            </div>
                            <h3 class="text-xl font-semibold text-gray-900">Project Management</h3>
                        </div>
                        <p class="mt-4 text-gray-600">Skilled in leading consulting projects, delivering solutions efficiently, and stakeholder communication.</p>
                        <ul class="mt-4 space-y-2 text-sm text-gray-500 list-disc list-inside">
                            <li>Scrum/Agile Principles</li>
                            <li>Stakeholder Management</li>
                        </ul>
                    </div>

                    <!-- Skill Card 3 -->
                    <div class="p-6 bg-white rounded-xl shadow-2xl transition duration-500 transform hover:shadow-exl-blue/30 hover:-translate-y-1">
                        <div class="flex items-center space-x-4">
                            <div class="flex-shrink-0 bg-exl-blue text-white rounded-full p-3">
                                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8c1.657 0 3 .895 3 2s-1.343 2-3 2-3-.895-3-2 1.343-2 3-2z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 14c-1.657 0-3 1.105-3 2.5v1.5h6v-1.5c0-1.395-1.343-2.5-3-2.5z"></path></svg>
                            </div>
                            <h3 class="text-xl font-semibold text-gray-900">Personal & Financial</h3>
                        </div>
                        <p class="mt-4 text-gray-600">A disciplined approach to personal finance, health, and self-learning (Japanese, Guitar, Swimming).</p>
                        <ul class="mt-4 space-y-2 text-sm text-gray-500 list-disc list-inside">
                            <li>Expense/Budget Tracking (Sheets)</li>
                            <li>Long-term Investment Planning</li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <!-- 3. Goals Section (Personalized to User's Ambitions) -->
        <section id="goals" class="py-20 bg-white border-b border-gray-200">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center">
                    <h2 class="text-3xl font-extrabold text-gray-900 sm:text-4xl">Current Focus Areas</h2>
                    <p class="mt-4 text-lg text-gray-500">
                        Tracking consistency across health, finance, and learning objectives.
                    </p>
                </div>

                <div class="mt-12 grid grid-cols-1 md:grid-cols-2 gap-12">
                    <!-- Goal Area: Health & Fitness -->
                    <div>
                        <h3 class="text-2xl font-bold text-exl-blue border-b-2 border-fms-gold pb-2 mb-6 flex items-center">
                            <svg class="w-6 h-6 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"></path></svg>
                            Health & Wellness
                        </h3>
                        <ul class="space-y-4">
                            <li class="p-4 bg-gray-50 rounded-lg shadow-md">
                                <span class="font-semibold text-gray-900">Weight Gain:</span> Target 56 kg (Current focus: consistency, calorie tracking).
                            </li>
                            <li class="p-4 bg-gray-50 rounded-lg shadow-md">
                                <span class="font-semibold text-gray-900">Fitness:</span> Consistent Badminton, Running, and starting Swimming.
                            </li>
                            <li class="p-4 bg-gray-50 rounded-lg shadow-md">
                                <span class="font-semibold text-gray-900">Habits:</span> Optimize sleep and eating habits.
                            </li>
                        </ul>
                    </div>

                    <!-- Goal Area: Learning & Finance -->
                    <div>
                        <h3 class="text-2xl font-bold text-exl-blue border-b-2 border-fms-gold pb-2 mb-6 flex items-center">
                            <svg class="w-6 h-6 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6.253v13m0-13C10.832 5.477 9.206 5 7.5 5S4.168 5.477 3 6.253v13C4.168 18.477 5.794 18 7.5 18s3.332.477 4.5 1.253m0-13C13.168 5.477 14.794 5 16.5 5s3.332.477 4.5 1.253v13C19.832 18.477 18.206 18 16.5 18s-3.332.477-4.5 1.253"></path></svg>
                            Finance & Skills
                        </h3>
                        <ul class="space-y-4">
                            <li class="p-4 bg-gray-50 rounded-lg shadow-md">
                                <span class="font-semibold text-gray-900">Automation:</span> Automate monthly investments and expense tracking.
                            </li>
                            <li class="p-4 bg-gray-50 rounded-lg shadow-md">
                                <span class="font-semibold text-gray-900">Learning:</span> Progress in Japanese, Chess, and Guitar.
                            </li>
                            <li class="p-4 bg-gray-50 rounded-lg shadow-md">
                                <span class="font-semibold text-gray-900">Financial Visibility:</span> Maintain clear tracking of income, EMIs, and savings.
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <!-- 4. Contact Section -->
        <section id="contact" class="py-20 bg-gray-50">
            <div class="max-w-xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center">
                    <h2 class="text-3xl font-extrabold text-gray-900 sm:text-4xl">Get In Touch</h2>
                    <p class="mt-4 text-lg text-gray-500">
                        Let's connect on professional opportunities or collaborative projects.
                    </p>
                </div>
                
                <div class="mt-12 bg-white p-8 rounded-xl shadow-2xl">
                    <form id="contact-form" class="space-y-6">
                        <div>
                            <label for="name" class="block text-sm font-medium text-gray-700">Name</label>
                            <input type="text" id="name" required class="mt-1 block w-full border-gray-300 rounded-lg shadow-sm focus:ring-exl-blue focus:border-exl-blue p-3 border">
                        </div>
                        <div>
                            <label for="email" class="block text-sm font-medium text-gray-700">Email</label>
                            <input type="email" id="email" required class="mt-1 block w-full border-gray-300 rounded-lg shadow-sm focus:ring-exl-blue focus:border-exl-blue p-3 border">
                        </div>
                        <div>
                            <label for="message" class="block text-sm font-medium text-gray-700">Message</label>
                            <textarea id="message" rows="4" required class="mt-1 block w-full border-gray-300 rounded-lg shadow-sm focus:ring-exl-blue focus:border-exl-blue p-3 border"></textarea>
                        </div>
                        <div id="status-message" class="text-center p-3 text-sm rounded-lg transition-all duration-300 hidden"></div>
                        <button type="submit" class="w-full flex justify-center py-3 px-4 border border-transparent rounded-xl shadow-sm text-base font-medium text-white bg-fms-gold hover:bg-amber-600 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-fms-gold transition duration-300 transform hover:scale-[1.01]">
                            Send Message
                        </button>
                    </form>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white">
        <div class="max-w-7xl mx-auto py-8 px-4 sm:px-6 lg:px-8 text-center">
            <p class="text-sm">&copy; 2025 Mihir. Built with structure and clarity.</p>
            <div class="mt-4 flex justify-center space-x-6">
                <a href="#home" class="text-gray-400 hover:text-white transition duration-300">Back to Top</a>
            </div>
        </div>
    </footer>

    <!-- JavaScript for Interactivity -->
    <script>
        // Function to toggle the mobile menu visibility
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Function to close the mobile menu when a link is clicked
        function closeMobileMenu() {
            mobileMenu.classList.add('hidden');
        }

        // Simple form submission handler (since we cannot send data to a server)
        const contactForm = document.getElementById('contact-form');
        const statusMessage = document.getElementById('status-message');

        contactForm.addEventListener('submit', function(event) {
            event.preventDefault(); // Stop the form from performing its default submission
            
            // Get form values
            const name = document.getElementById('name').value;
            
            // Simulate form submission success
            statusMessage.classList.remove('hidden', 'bg-red-100', 'text-red-700');
            statusMessage.classList.add('bg-green-100', 'text-green-700');
            statusMessage.textContent = `Thank you, ${name}! Your message has been received. I'll connect with you shortly.`;

            // Reset the form after a delay
            setTimeout(() => {
                contactForm.reset();
                statusMessage.classList.add('hidden');
            }, 5000);
        });
    </script>
</body>
</html>
