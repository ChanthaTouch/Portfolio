<template>
  <div class="bg-gray-900 text-white min-h-screen font-sans">
    <!-- Hero Section with Background Image -->
    <header class="relative h-screen flex flex-col items-center justify-center text-center px-6 md:px-12 bg-cover bg-center" style="background-image: url('./assets//');">
      <div class="absolute inset-0 bg-black opacity-60"></div>
      <div class="relative z-10">
        <img
          src="./assets/chantha.jpg"
          alt="Chantha Touch"
          class="rounded-full shadow-lg border-4 border-blue-400 w-40 h-40 object-cover mx-auto mb-6"
        />
        <p class="text-xl font-medium text-blue-400">Hello, I'm</p>
        <h1 class="text-5xl md:text-7xl font-bold mt-2">Chantha Touch</h1>
        <h2 class="text-3xl md:text-4xl font-semibold text-gray-300 mt-2">A Full-Stack Developer</h2>
        <p class="mt-4 max-w-xl mx-auto text-gray-400">
          A dedicated Computer Science student at the Royal University of Phnom Penh, focused on building robust and intuitive web applications.
        </p>

        <!-- Social Icons -->
        <div class="flex justify-center space-x-4 mt-6">
          <a href="#" class="p-3 bg-gray-800 rounded-full hover:bg-blue-400 transition-colors duration-300">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-twitter text-white"><path d="M22 4s-.7 2.1-2 3.4c-.7.9-2.5 2.1-4 2.3 0 1.5.3 2.5.3 3.6 0 5.1-3.2 8.4-9.3 8.4C4.3 21.7 1 20 1 20s3.4-1.2 5-3c1.7-.8 3-2.6 3.7-4.5.3-1.1.6-2.5-.3-3.6 0 0-1.8-1.7-2.3-3.1C6 4.7 7.5 3 9.4 3c1.9 0 3.6 1.4 4.5 2.5.8.1 1.7.5 2.5 1.1 0 0 1.5-.7 2.7-1.3 0 0-.6 1.7-1.1 2.9.8.1 1.6.4 2.3.8z"></path></svg>
          </a>
          <a href="#" class="p-3 bg-gray-800 rounded-full hover:bg-red-500 transition-colors duration-300">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-youtube text-white"><path d="M2.5 17.5a2.5 2.5 0 0 1-2.5-2.5v-5a2.5 2.5 0 0 1 2.5-2.5h19a2.5 2.5 0 0 1 2.5 2.5v5a2.5 2.5 0 0 1-2.5 2.5z"></path><path d="M10 9l5 3-5 3v-6z"></path></svg>
          </a>
          <a href="#" class="p-3 bg-gray-800 rounded-full hover:bg-blue-600 transition-colors duration-300">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-facebook text-white"><path d="M18 2h-3a5 5 0 00-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 011-1h3z"></path></svg>
          </a>
          <a href="#" class="p-3 bg-gray-800 rounded-full hover:bg-pink-600 transition-colors duration-300">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-instagram text-white"><rect width="20" height="20" x="2" y="2" rx="5" ry="5"></rect><path d="M16 11.37a4 4 0 11-4-4"></path><line x1="17.5" x2="17.51" y1="6.5" y2="6.5"></line></svg>
          </a>
        </div>

      </div>
    </header>

    <!-- About Me Section -->
    <section class="py-16 bg-gray-800">
      <div class="container mx-auto px-6 md:px-12 text-center">
        <h2 class="text-3xl font-bold border-b-2 border-blue-400 pb-2 mb-8 inline-block">About Me</h2>
        <div class="max-w-3xl mx-auto text-gray-300 leading-relaxed">
          <p class="mb-4">
            I am a passionate and results-driven computer science student at the Royal University of Phnom Penh. I specialize in full-stack development, blending front-end technologies with back-end solutions to create seamless and effective digital experiences.
          </p>
          <p>
            My goal is to leverage my skills in VUE.js, React.js, and Laravel to build innovative and scalable applications that solve real-world problems.
          </p>
        </div>
      </div>
    </section>

    <!-- Skills Section -->
    <section class="py-16">
      <div class="container mx-auto px-6 md:px-12 text-center">
        <h2 class="text-3xl font-bold border-b-2 border-blue-400 pb-2 mb-8 inline-block">Skills</h2>
        <div class="flex flex-wrap justify-center gap-4">
          <span v-for="skill in skills" :key="skill" class="bg-blue-400 text-gray-900 text-sm font-semibold px-4 py-2 rounded-full shadow-md hover:scale-105 transition-transform duration-200">
            {{ skill }}
          </span>
        </div>
      </div>
    </section>

    <!-- Contact Section -->
    <section class="py-16 bg-gray-800">
      <div class="container mx-auto px-6 md:px-12 text-center">
        <h2 class="text-3xl font-bold border-b-2 border-blue-400 pb-2 mb-8 inline-block">Contact Me</h2>
        <div class="flex flex-col items-center max-w-md mx-auto space-y-4 text-gray-300">
          <div class="flex items-center space-x-3">
            <span class="p-2 rounded-full bg-blue-400 text-gray-900">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                <path d="M2.003 5.884L10 9.882l7.997-3.998A2 2 0 0016 4H4a2 2 0 00-1.997 1.884z" />
                <path d="M18 8.118l-8 4-8-4V14a2 2 0 002 2h12a2 2 0 002-2V8.118z" />
              </svg>
            </span>
            <a href="mailto:tchantha2004@gmail.com" class="hover:underline text-blue-400">tchantha2004@gmail.com</a>
          </div>
          <div class="flex items-center space-x-3">
            <span class="p-2 rounded-full bg-blue-400 text-gray-900">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                <path d="M2 3a1 1 0 011-1h2.153a1 1 0 01.986.836l.743 4.458A1 1 0 017.5 9h-1.892a1 1 0 00-.992 1.155l.775 4.65a1 1 0 00.992.845H12a1 1 0 00.992-.845l.775-4.65a1 1 0 00-.992-1.155H12a1 1 0 01-1-1v-.966a1 1 0 011.025-.992l1.378-.23c.365-.06.758.077.954.385l.593.916a1 1 0 001.378.11l1.894-1.263a1 1 0 00.505-.875V3a1 1 0 011-1h1.5a1 1 0 011 1v14a1 1 0 01-1 1h-1.5a1 1 0 01-1-1v-2.5a1 1 0 00-.992-1.155l-.775-4.65a1 1 0 00-1-1.155H8a1 1 0 00-1 1v.966a1 1 0 01-1 1H5.5a1 1 0 01-1-1v-2.5z" />
              </svg>
            </span>
            <p>0966463091</p>
          </div>
          <div class="flex items-center space-x-3">
            <span class="p-2 rounded-full bg-blue-400 text-gray-900">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM4.332 7.643A4 4 0 0110 4.172v3.471l-5.668-2.61zM10 15.828V12.356l5.668 2.61A4 4 0 0110 15.828zM15.668 7.643L10 5.035V8.506l5.668-2.61zM4.332 12.357L10 14.965v-3.471l-5.668 2.61z" clip-rule="evenodd" />
                <path d="M10 18a8 8 0 100-16 8 8 0 000 16zm-5.668-2.61A4 4 0 0110 4.172v3.471l-5.668-2.61zM10 15.828V12.356l5.668 2.61A4 4 0 0110 15.828zm5.668-8.185L10 5.035V8.506l5.668-2.61zM4.332 12.357L10 14.965v-3.471l-5.668 2.61z" />
              </svg>
            </span>
            <a href="https://t.me/Touchh_Chantha" target="_blank" class="hover:underline text-blue-400">Telegram Account</a>
          </div>
          <div class="flex items-center space-x-3">
            <span class="p-2 rounded-full bg-blue-400 text-gray-900">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                <path fill-rule="evenodd" d="M5.05 4.05a7 7 0 119.9 9.9L10 18.9l-4.95-4.95a7 7 0 010-9.9zM10 11a2 2 0 100-4 2 2 0 000 4z" clip-rule="evenodd" />
              </svg>
            </span>
            <p>Sangkat Teuk Thla, Khan Sen Sok, Phnom Penh</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-950 text-gray-500 text-center p-6">
      <p>&copy; 2024 Chantha Touch. All rights reserved.</p>
    </footer>

  </div>
</template>

<script setup>
import { ref } from 'vue';

const skills = ref([
  'Vue.js', 'React.js', 'JavaScript', 'Tailwind CSS', 'CSS 3',
  'Bootstrap 3', 'Laravel', 'PHP', 'MySQL', 'Server', 'Github'
]);
</script>
