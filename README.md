# Personal-Portfolio
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lilesh Humane | Software Developer</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        
        body {
            font-family: 'Poppins', sans-serif;
            background: #FFFFFF;
            color: #1E1E1E;
        }
        
        .nav-link {
            position: relative;
        }
        
        .nav-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -4px;
            left: 0;
            background-color: #3b82f6;
            transition: width 0.3s ease;
        }
        
        .nav-link:hover::after {
            width: 100%;
        }
        
        .profile-img {
            animation: float 3s ease-in-out infinite;
        }
        
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
            100% { transform: translateY(0px); }
        }
        
        .tech-icon {
            transition: all 0.3s ease;
        }
        
        .tech-icon:hover {
            transform: translateY(-5px);
        }
        
        .project-card {
            transition: all 0.3s ease;
        }
        
        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
        
        .experience-card {
            position: relative;
        }
        
        .experience-card::before {
            content: '';
            position: absolute;
            width: 4px;
            height: 100%;
            left: -20px;
            background: #3b82f6;
            border-radius: 20px;
        }
        
        .fade-in {
            animation: fadeIn 1s ease-in;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        section {
            scroll-margin-top: 80px;
        }
    </style>
</head>
<body>
    <!-- Header/Navigation -->
    <header class="fixed w-full bg-white shadow-md z-50">
        <div class="container mx-auto px-6 py-3">
            <div class="flex items-center justify-between">
                <a href="#" class="text-2xl font-bold text-blue-500">Lilesh<span class="text-gray-800">Humane</span></a>
                
                <nav class="hidden md:flex space-x-8">
                    <a href="#home" class="nav-link text-gray-700 hover:text-blue-500">Home</a>
                    <a href="#about" class="nav-link text-gray-700 hover:text-blue-500">About</a>
                    <a href="#projects" class="nav-link text-gray-700 hover:text-blue-500">Projects</a>
                    <a href="#experience" class="nav-link text-gray-700 hover:text-blue-500">Experience</a>
                </nav>
                
                <!-- Mobile menu button -->
                <button id="mobile-menu-button" class="md:hidden text-gray-700 focus:outline-none">
                    <i class="fas fa-bars text-xl"></i>
                </button>
            </div>
            
            <!-- Mobile menu -->
            <div id="mobile-menu" class="hidden md:hidden mt-4 pb-4">
                <a href="#home" class="block py-2 text-gray-700 hover:text-blue-500">Home</a>
                <a href="#about" class="block py-2 text-gray-700 hover:text-blue-500">About</a>
                <a href="#projects" class="block py-2 text-gray-700 hover:text-blue-500">Projects</a>
                <a href="#experience" class="block py-2 text-gray-700 hover:text-blue-500">Experience</a>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="home" class="pt-32 pb-16 md:pt-40 md:pb-20">
        <div class="container mx-auto px-6 flex flex-col-reverse md:flex-row items-center">
            <div class="md:w-1/2 mt-10 md:mt-0 fade-in">
                <h1 class="text-4xl md:text-5xl font-bold text-gray-800">Hi, I'm <span class="text-blue-500">Lilesh Humane</span></h1>
                <h2 class="text-2xl md:text-3xl text-gray-600 mt-2">Software Developer</h2>
                <p class="text-gray-600 mt-4 mb-8 leading-relaxed">I build exceptional digital experiences with Java and modern web technologies.</p>
                
                <div class="flex flex-wrap gap-4">
                    <a href="#contact" class="bg-blue-500 hover:bg-blue-600 text-white px-6 py-3 rounded-lg font-medium transition duration-300 transform hover:scale-105">Contact Me</a>
                    <a href="#" class="border border-blue-500 text-blue-500 hover:bg-blue-50 px-6 py-3 rounded-lg font-medium transition duration-300 transform hover:scale-105">Download CV</a>
                </div>
                
                <div class="flex mt-10 space-x-4">
                    <a href="#" class="text-gray-600 hover:text-blue-500 transition duration-300">
                        <i class="fab fa-github text-2xl"></i>
                    </a>
                    <a href="#" class="text-gray-600 hover:text-blue-500 transition duration-300">
                        <i class="fab fa-linkedin text-2xl"></i>
                    </a>
                </div>
            </div>
            
            <div class="md:w-1/2 flex justify-center fade-in">
                <div class="profile-img relative">
                    <div class="absolute -inset-4 bg-blue-500 rounded-full opacity-20 animate-pulse"></div>
                    <img src="https://via.placeholder.com/400x400" alt="Lilesh Humane" class="rounded-full w-64 h-64 md:w-80 md:h-80 object-cover border-4 border-white shadow-xl">
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-16 bg-white fade-in">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-12">About <span class="text-blue-500">Me</span></h2>
            
            <div class="md:flex items-center">
                <div class="md:w-1/2 mb-10 md:mb-0 md:pr-10">
                    <h3 class="text-2xl font-semibold text-gray-800 mb-4">Who am I?</h3>
                    <p class="text-gray-600 leading-relaxed mb-6">
                        I'm Lilesh Humane, a passionate software developer with expertise in Java and web development.
                        I completed my degree in Computer Science and have hands-on experience from both a 6-month 
                        and a 1-month internship in software development.
                    </p>
                    <p class="text-gray-600 leading-relaxed mb-6">
                        During my internships, I worked on real-world projects that gave me valuable experience in 
                        Java development, debugging, and collaborating in a professional environment. I'm eager 
                        to apply my skills and continue learning as I start my professional career.
                    </p>
                    <p class="text-gray-600 leading-relaxed">
                        When I'm not coding, I enjoy staying updated with the latest technologies through tech blogs,
                        and working on personal projects to enhance my skills.
                    </p>
                    
                    <div class="mt-8">
                        <a href="#contact" class="bg-blue-500 hover:bg-blue-600 text-white px-6 py-3 rounded-lg font-medium">Get In Touch</a>
                    </div>
                </div>
                
                <div class="md:w-1/2">
                    <h3 class="text-2xl font-semibold text-gray-800 mb-6">My Skills</h3>
                    
                    <div class="mb-8">
                        <h4 class="text-lg font-medium text-gray-700 mb-4">Java Development</h4>
                        <div class="w-full bg-gray-200 rounded-full h-2.5">
                            <div class="bg-blue-500 h-2.5 rounded-full" style="width: 90%"></div>
                        </div>
                    </div>
                    
                    <div class="mb-8">
                        <h4 class="text-lg font-medium text-gray-700 mb-4">Spring Framework</h4>
                        <div class="w-full bg-gray-200 rounded-full h-2.5">
                            <div class="bg-blue-500 h-2.5 rounded-full" style="width: 85%"></div>
                        </div>
                    </div>
                    
                    <div class="mb-8">
                        <h4 class="text-lg font-medium text-gray-700 mb-4">JavaScript</h4>
                        <div class="w-full bg-gray-200 rounded-full h-2.5">
                            <div class="bg-blue-500 h-2.5 rounded-full" style="width: 80%"></div>
                        </div>
                    </div>
                    
                    <div class="mb-8">
                        <h4 class="text-lg font-medium text-gray-700 mb-4">HTML/CSS</h4>
                        <div class="w-full bg-gray-200 rounded-full h-2.5">
                            <div class="bg-blue-500 h-2.5 rounded-full" style="width: 85%"></div>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Technologies I Work With -->
            <div class="mt-16">
                <h3 class="text-2xl font-semibold text-center text-gray-800 mb-12">Technologies I Work With</h3>
                
                <div class="grid grid-cols-3 md:grid-cols-6 gap-6 text-center">
                    <div class="tech-icon">
                        <i class="fab fa-java text-6xl text-gray-700 mb-2"></i>
                        <p class="text-gray-600">Java</p>
                    </div>
                    <div class="tech-icon">
                        <i class="fab fa-js-square text-6xl text-yellow-300 mb-2"></i>
                        <p class="text-gray-600">JavaScript</p>
                    </div>
                    <div class="tech-icon">
                        <i class="fab fa-html5 text-6xl text-orange-500 mb-2"></i>
                        <p class="text-gray-600">HTML5</p>
                    </div>
                    <div class="tech-icon">
                        <i class="fab fa-css3-alt text-6xl text-blue-500 mb-2"></i>
                        <p class="text-gray-600">CSS3</p>
                    </div>
                    <div class="tech-icon">
                        <i class="fab fa-react text-6xl text-blue-400 mb-2"></i>
                        <p class="text-gray-600">React</p>
                    </div>
                    <div class="tech-icon">
                        <i class="fas fa-database text-6xl text-gray-600 mb-2"></i>
                        <p class="text-gray-600">SQL</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="py-16 fade-in">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-4">My <span class="text-blue-500">Projects</span></h2>
            <p class="text-gray-600 text-center max-w-2xl mx-auto mb-12">Academic and personal projects demonstrating my learning journey in software development.</p>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Project 1 -->
                <div class="project-card bg-white rounded-xl shadow-md overflow-hidden transform hover:shadow-xl">
                    <div class="h-48 bg-blue-500 flex items-center justify-center">
                        <i class="fas fa-project-diagram text-6xl text-white"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold text-gray-800 mb-2">Student Management System</h3>
                        <p class="text-gray-600 mb-4">A simple Java CRUD application for managing student records.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Java</span>
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Spring Boot</span>
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">React</span>
                        </div>
                        <div class="flex space-x-3">
                            <a href="#" class="text-blue-500 hover:text-blue-700 font-medium">View Project</a>
                            <a href="#" class="text-gray-500 hover:text-gray-700 font-medium">View Code</a>
                        </div>
                    </div>
                </div>
                
                <!-- Project 2 -->
                <div class="project-card bg-white rounded-xl shadow-md overflow-hidden transform hover:shadow-xl">
                    <div class="h-48 bg-green-500 flex items-center justify-center">
                        <i class="fas fa-chart-line text-6xl text-white"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold text-gray-800 mb-2">Portfolio Website</h3>
                        <p class="text-gray-600 mb-4">A responsive personal portfolio built with HTML, CSS and JavaScript.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Java</span>
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Python</span>
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">D3.js</span>
                        </div>
                        <div class="flex space-x-3">
                            <a href="#" class="text-blue-500 hover:text-blue-700 font-medium">View Project</a>
                            <a href="#" class="text-gray-500 hover:text-gray-700 font-medium">View Code</a>
                        </div>
                    </div>
                </div>
                
                <!-- Project 3 -->
                <div class="project-card bg-white rounded-xl shadow-md overflow-hidden transform hover:shadow-xl">
                    <div class="h-48 bg-purple-500 flex items-center justify-center">
                        <i class="fas fa-blog text-6xl text-white"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold text-gray-800 mb-2">Temperature Converter</h3>
                        <p class="text-gray-600 mb-4">A simple Java GUI application to convert between Celsius and Fahrenheit.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Java</span>
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Spring</span>
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Thymeleaf</span>
                        </div>
                        <div class="flex space-x-3">
                            <a href="#" class="text-blue-500 hover:text-blue-700 font-medium">View Project</a>
                            <a href="#" class="text-gray-500 hover:text-gray-700 font-medium">View Code</a>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-12">
                <a href="#" class="inline-block border border-blue-500 text-blue-500 hover:bg-blue-50 px-6 py-3 rounded-lg font-medium">View All Projects</a>
            </div>
        </div>
    </section>

    <!-- Experience Section -->
    <section id="experience" class="py-16 bg-white fade-in">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-12">Work <span class="text-blue-500">Experience</span></h2>
            
            <div class="max-w-3xl mx-auto">
                <!-- Internship 1 -->
                <div class="experience-card bg-white p-6 rounded-lg shadow-md mb-6 relative">
                    <div class="flex flex-col md:flex-row md:justify-between mb-4">
                        <h3 class="text-xl font-bold text-gray-800">Software Developer Intern</h3>
                        <span class="text-blue-500 font-medium">Jun 2025 - Dec 2025</span>
                    </div>
                    <h4 class="text-lg font-semibold text-gray-700 mb-2">TechCiti Software Consulting Pvt Ltd</h4>
                    <p class="text-gray-600 mb-4">
                        Six-month internship focusing on Java development and web technologies.
                        Contributed to real-world projects and enhanced my professional skills.
                    </p>
                    <ul class="list-disc text-gray-600 pl-5 space-y-1">
                        <li>Developed Java applications under senior developer guidance</li>
                        <li>Collaborated on Spring Boot projects</li>
                        <li>Participated in code reviews and agile processes</li>
                    </ul>
                </div>

                <!-- Internship 2 -->
                <div class="experience-card bg-white p-6 rounded-lg shadow-md mb-6 relative">
                    <div class="flex flex-col md:flex-row md:justify-between mb-4">
                        <h3 class="text-xl font-bold text-gray-800">Software Developer Intern</h3>
                        <span class="text-blue-500 font-medium">Mar 1, 2025 - Mar 31, 2025</span>
                    </div>
                    <h4 class="text-lg font-semibold text-gray-700 mb-2">SkillCraft Technology</h4>
                    <p class="text-gray-600 mb-4">
                        One-month intensive internship where I learned the fundamentals of software development
                        processes and contributed to small-scale projects.
                    </p>
                    <ul class="list-disc text-gray-600 pl-5 space-y-1">
                        <li>Assisted in debugging and testing applications</li>
                        <li>Learned software development best practices</li>
                        <li>Worked on small feature implementations</li>
                    </ul>
                </div>

            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-16 fade-in">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-4">Get In <span class="text-blue-500">Touch</span></h2>
            <p class="text-gray-600 text-center max-w-2xl mx-auto mb-12">Have a project in mind or want to discuss potential opportunities? Feel free to reach out!</p>
            
            <div class="max-w-4xl mx-auto bg-white rounded-xl shadow-md overflow-hidden">
                <div class="md:flex">
                    <div class="md:w-1/2 bg-blue-500 text-white p-8">
                        <h3 class="text-2xl font-bold mb-6">Contact Information</h3>
                        <div class="space-y-6">
                            <div class="flex items-start">
                                <i class="fas fa-envelope mt-1 mr-4"></i>
                                <div>
                                    <h4 class="font-semibold mb-1">Email</h4>
                                    <p class="text-blue-100">lileshhumane@gmail.com</p>
                                </div>
                            </div>
                            <div class="flex items-start">
                                <i class="fas fa-phone-alt mt-1 mr-4"></i>
                                <div>
                                    <h4 class="font-semibold mb-1">Phone</h4>
                                    <p class="text-blue-100">+91 88304 34051</p>
                                </div>
                            </div>
                            <div class="flex items-start">
                                <i class="fas fa-map-marker-alt mt-1 mr-4"></i>
                                <div>
                                    <h4 class="font-semibold mb-1">Location</h4>
                                    <p class="text-blue-100">Nagpur, India</p>
                                </div>
                            </div>
                        </div>
                        
                        <div class="mt-12">
                            <h3 class="text-2xl font-bold mb-6">Connect With Me</h3>
                            <div class="flex space-x-4">
                                <a href="#" class="bg-blue-600 hover:bg-blue-700 w-10 h-10 rounded-full flex items-center justify-center transition duration-300">
                                    <i class="fab fa-github"></i>
                                </a>
                                <a href="#" class="bg-blue-600 hover:bg-blue-700 w-10 h-10 rounded-full flex items-center justify-center transition duration-300">
                                    <i class="fab fa-linkedin-in"></i>
                                </a>
                            </div>
                        </div>
                    </div>
                    
                    <div class="md:w-1/2 p-8">
                        <form>
                            <div class="mb-6">
                                <label for="name" class="block text-gray-700 font-medium mb-2">Your Name</label>
                                <input type="text" id="name" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 outline-none transition duration-300" placeholder="John Doe">
                            </div>
                            <div class="mb-6">
                                <label for="email" class="block text-gray-700 font-medium mb-2">Your Email</label>
                                <input type="email" id="email" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 outline-none transition duration-300" placeholder="john@example.com">
                            </div>
                            <div class="mb-6">
                                <label for="subject" class="block text-gray-700 font-medium mb-2">Subject</label>
                                <input type="text" id="subject" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 outline-none transition duration-300" placeholder="Let's talk about">
                            </div>
                            <div class="mb-6">
                                <label for="message" class="block text-gray-700 font-medium mb-2">Message</label>
                                <textarea id="message" rows="4" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 outline-none transition duration-300" placeholder="Your message here..."></textarea>
                            </div>
                            <button type="submit" class="w-full bg-blue-500 hover:bg-blue-600 text-white px-6 py-3 rounded-lg font-medium transition duration-300">Send Message</button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-black text-white py-8">
        <div class="container mx-auto px-6">
            <div class="flex flex-col items-center">
                <h2 class="text-2xl font-bold mb-4">Lilesh Humane</h2>
                <p class="text-gray-400 mb-6 text-center max-w-2xl">Software Developer passionate about creating efficient and user-friendly digital experiences.</p>
                
                <div class="flex space-x-6 mb-6">
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300">
                        <i class="fab fa-github text-xl"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300">
                        <i class="fab fa-linkedin-in text-xl"></i>
                    </a>
                </div>
                
                <div class="flex flex-wrap justify-center space-x-6 mb-6">
                    <a href="#home" class="text-gray-400 hover:text-white transition duration-300">Home</a>
                    <a href="#about" class="text-gray-400 hover:text-white transition duration-300">About</a>
                    <a href="#projects" class="text-gray-400 hover:text-white transition duration-300">Projects</a>
                    <a href="#experience" class="text-gray-400 hover:text-white transition duration-300">Experience</a>
                    <a href="#contact" class="text-gray-400 hover:text-white transition duration-300">Contact</a>
                </div>
                
                <p class="text-gray-500 text-sm">© 2023 Lilesh Humane. All rights reserved.</p>
            </div>
        </div>
    </footer>
    
    <!-- Back to Top Button -->
    <button id="back-to-top" class="fixed bottom-8 right-8 bg-blue-500 text-white w-12 h-12 rounded-full shadow-lg hidden items-center justify-center transition duration-300 hover:bg-blue-600">
        <i class="fas fa-arrow-up"></i>
    </button>
    
    <script>
        // Mobile menu toggle
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');
        
        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
        
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                
                window.scrollTo({
                    top: targetElement.offsetTop - 80,
                    behavior: 'smooth'
                });
                
                // Close mobile menu if open
                if (!mobileMenu.classList.contains('hidden')) {
                    mobileMenu.classList.add('hidden');
                }
            });
        });
        
        // Back to top button
        const backToTopButton = document.getElementById('back-to-top');
        
        window.addEventListener('scroll', () => {
            if (window.scrollY > 300) {
                backToTopButton.classList.remove('hidden');
                backToTopButton.classList.add('flex');
            } else {
                backToTopButton.classList.add('hidden');
                backToTopButton.classList.remove('flex');
            }
        });
        
        backToTopButton.addEventListener('click', () => {
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });
        
        // Intersection Observer for fade-in animations
        const fadeElements = document.querySelectorAll('.fade-in');
        
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('animate-fadeIn');
                }
            });
        }, {
            threshold: 0.1
        });
        
        fadeElements.forEach(element => {
            observer.observe(element);
        });
    </script>
</body>
</html>
