<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Archita | Portfolio</title>
<script src="https://cdn.tailwindcss.com"></script>
<script>
document.addEventListener('DOMContentLoaded', () => {
const texts = ["Frontend Developer", "UI/UX Enthusiast", "Tailwind CSS Lover"];
let count = 0;
let index = 0;
let currentText = '';
let letter = '';

(function type() {
if (count === texts.length) count = 0;
currentText = texts[count];
letter = currentText.slice(0, ++index);
document.getElementById('typing').textContent = letter;
if (letter.length === currentText.length) {
count++;
index = 0;
setTimeout(type, 1000);
} else {
setTimeout(type, 100);
}
})();
});
</script>
</head>
<body class="bg-pink-100 text-gray-800 font-sans">

<!-- Navbar -->
<header class="bg-gray-900 text-white p-4 sticky top-0 z-50">
<nav class="max-w-7xl mx-auto flex justify-between items-center">
<h1 class="text-xl font-bold">Archita</h1>
<ul class="flex gap-6">
<li><a href="#home" class="hover:text-yellow-400">Home</a></li>
<li><a href="#about" class="hover:text-yellow-400">About</a></li>
<li><a href="#projects" class="hover:text-yellow-400">Projects</a></li>
<li><a href="#contact" class="hover:text-yellow-400">Contact</a></li>
</ul>
</nav>
</header>

<!-- Home Section -->
<section id="home" class="min-h-screen flex flex-col justify-center items-center text-center px-6">
<img src="images/your-photo.jpg" alt="Archita's Photo" class="w-40 h-40 rounded-full mb-4" />
<h2 class="text-3xl font-bold mb-2" style="font-style: italic;text-shadow: 2px 2px 2px red ;" >Hi, I'm Archita</h2>

<p class="text-xl text-gray-600 mb-4"><span id="typing"></span></p>
<a href="images/resume.pdf" class="bg-yellow-400 px-4 py-2 rounded hover:bg-yellow-500 transition" download >Download Resume</a>
</section>

<!-- About Me Section -->
<section id="about" class="bg-blue-100 py-16 px-6">
<div class="max-w-4xl mx-auto">
<h2 class="text-2xl font-bold mb-6" style="color: red;">About Me</h2>
<p class="mb-4" style="font-style: italic;">I'm a 3rd-year Computer Science student at HMR Institute of Technology & Management, IPU. Passionate about development, analytics, and problem-solving.</p>
<div class="grid sm:grid-cols-2 gap-4">
<div>
<h3 class="font-semibold mb-2" style="color: blueviolet;">Skills</h3>
<ul class="list-disc list-inside">
<li>HTML, CSS, JavaScript</li>
<li>Python, MySQL, Java</li>
<li>Tailwind CSS</li>
<li>Tableau, Excel, Google BigQuery</li>
</ul>
</div>
<div>
<h3 class="font-semibold mb-2" style="color:blueviolet">Education & Experience</h3>
<ul class="list-disc list-inside">
<li>B.Tech CSE - HMRITM (IPU), 3rd Year, GPA 8.3</li>
<li>Intern - Data Analytics at Deloitte & Tata IQ (virtual)</li>
<li>Participant - Smart India Hackathon (SIH)</li>
</ul>
</div>
</div>
</div>
</section>

<!-- Projects Section -->
<section id="projects" class="bg-green-100 py-16 px-6">
<div class="max-w-5xl mx-auto">
<h2 class="text-2xl font-bold mb-6" style="color: blue;">Projects</h2>
<div class="grid md:grid-cols-3 gap-6">
<div class="bg-white shadow-md rounded-lg overflow-hidden transition transform hover:scale-105 hover:shadow-lg">
<img src="https://via.placeholder.com/300x150" alt="Sales Dashboard" class="w-full h-40 object-cover" />
<div class="p-4">
<h3 class="font-semibold text-lg mb-2" ">Sales Data Dashboard</h3>
<p class="text-sm text-gray-600 mb-2">Quarterly sales trends visualized in Tableau, supported with Excel-based insights.</p>
</div>
</div>
<div class="bg-white shadow-md rounded-lg overflow-hidden transition transform hover:scale-105 hover:shadow-lg">
<img src="https://via.placeholder.com/300x150" alt="E-Commerce Analysis" class="w-full h-40 object-cover" />
<div class="p-4">
<h3 class="font-semibold text-lg mb-2">E-Commerce Data Cleaning</h3>
<p class="text-sm text-gray-600 mb-2">Cleaned raw e-commerce data and analyzed behavior with Python, Pandas, NumPy.</p>
</div>
</div>
<div class="bg-white shadow-md rounded-lg overflow-hidden transition transform hover:scale-105 hover:shadow-lg">
<img src="https://via.placeholder.com/300x150" alt="Portfolio Website" class="w-full h-40 object-cover" />
<div class="p-4">
<h3 class="font-semibold text-lg mb-2">Portfolio Website</h3>
<p class="text-sm text-gray-600 mb-2">This very site – built with Tailwind CSS, showcasing all my awesomeness.</p>
</div>
</div>
</div>
</div>
</section>

<!-- Contact Section -->
<section id="contact" class="bg-violet-100 py-16 px-6">
<div class="max-w-md mx-auto">
<h2 class="text-2xl font-bold mb-6 text-center" style="color:purple" >Contact Me</h2>
<form class="space-y-4">
<input type="text" placeholder="Your Name" class="w-full border border-gray-300 p-2 rounded" />
<input type="email" placeholder="Your Email" class="w-full border border-gray-300 p-2 rounded" />
<textarea rows="4" placeholder="Your Message" class="w-full border border-gray-300 p-2 rounded"></textarea>
<button type="submit" class="bg-gray-900 text-white px-4 py-2 rounded hover:bg-gray-700">Send</button>
</form>
<div class="flex justify-center gap-4 mt-6">
<a href="https://github.com/" target="_blank"><img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/github.svg" class="w-6" alt="GitHub" /></a>
<a href="https://www.linkedin.com/in/archita-70a688316/" target="_blank"><img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/linkedin.svg" class="w-6" alt="LinkedIn" /></a>
</div>
</div>
</section>

<footer class="text-center py-4 text-sm text-gray-500">
&copy; 2025 Archita. All rights reserved.
</footer>
</body>
</html>
