<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Samir's Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#1E293B',
                        secondary: '#64748B'
                    }
                }
            }
        };
    </script>
    <script>
        function toggleDarkMode() {
            document.documentElement.classList.toggle('dark');
        }
    </script>
</head>
<body class="bg-gray-100 dark:bg-gray-900 text-gray-900 dark:text-gray-200">
    
    <!-- Navbar -->
  <nav class="fixed w-full bg-white dark:bg-gray-800 shadow-lg py-4 z-10">
        <div class="container mx-auto flex justify-between items-center px-6">
            <h1 class="text-xl font-bold">Samir</h1>
            <ul class="flex space-x-6">
                <li><a href="#about" class="hover:text-blue-500">About</a></li>
                <li><a href="#projects" class="hover:text-blue-500">Projects</a></li>
                <li><a href="#contact" class="hover:text-blue-500">Contact</a></li>
            </ul>
            <button onclick="toggleDarkMode()" class="px-4 py-2 bg-gray-300 dark:bg-gray-600 rounded">Dark Mode</button>
        </div>
    </nav>
    
    <!-- Hero Section -->
  <section id="home" class="h-screen flex flex-col justify-center items-center text-center">
        <h2 class="text-4xl font-bold">Hi, I'm Samir</h2>
        <p class="text-lg mt-2">A passionate AI & Data Science enthusiast</p>
        <a href="#projects" class="mt-4 px-6 py-3 bg-blue-500 text-white rounded">View My Work</a>
    </section>
    
    <!-- About Section -->
   <section id="about" class="py-16 px-6 text-center">
        <h2 class="text-3xl font-bold">About Me</h2>
        <p class="mt-4">I'm a data scientist and AI enthusiast, working on machine learning, deep learning, and web scraping projects.</p>
    </section>
    
    <!-- Projects Section -->
   <section id="projects" class="py-16 px-6 text-center bg-gray-200 dark:bg-gray-700">
        <h2 class="text-3xl font-bold">Projects</h2>
        <div class="mt-6 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
            <div class="p-4 bg-white dark:bg-gray-800 rounded shadow">Project 1</div>
            <div class="p-4 bg-white dark:bg-gray-800 rounded shadow">Project 2</div>
            <div class="p-4 bg-white dark:bg-gray-800 rounded shadow">Project 3</div>
        </div>
    </section>
    
    <!-- Contact Section -->
   <section id="contact" class="py-16 px-6 text-center">
        <h2 class="text-3xl font-bold">Contact</h2>
        <p class="mt-4">Reach out to me on <a href="#" class="text-blue-500">LinkedIn</a> or <a href="#" class="text-blue-500">GitHub</a></p>
    </section>
    
    <!-- Smooth Scroll -->
   <script>
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
