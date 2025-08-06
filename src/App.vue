<template>
  <div class="bg-gray-900 text-white min-h-screen font-sans">
    <!-- Hero Section with Background Image -->
    <header
      class="relative h-screen flex flex-col items-center justify-center text-center px-6 md:px-12 bg-cover bg-center"
      style="background-image: url('./assets/background.jpg');"
    >
      <div class="absolute inset-0 bg-black opacity-60"></div>
      <div class="relative z-10">
        <img
          src="./assets/profile.jpg"
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
            <i class="fab fa-linkedin"></i>
          </a>
          <a href="#" class="p-3 bg-gray-800 rounded-full hover:bg-red-500 transition-colors duration-300">
            <i class="fab fa-facebook-f"></i>
          </a>
          <a href="#" class="p-3 bg-gray-800 rounded-full hover:bg-blue-600 transition-colors duration-300">
            <i class="fab fa-instagram"></i>
          </a>
          <a href="#" class="p-3 bg-gray-800 rounded-full hover:bg-pink-600 transition-colors duration-300">
            <i class="fab fa-twitter"></i>
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
          <span
            v-for="skill in skills"
            :key="skill.name"
            class="flex items-center bg-blue-400 text-gray-900 text-sm font-semibold px-4 py-2 rounded-full shadow-md hover:scale-105 transition-transform duration-200"
          >
            <i :class="skill.icon" class="mr-2"></i>
            {{ skill.name }}
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
              <i class="fas fa-envelope"></i>
            </span>
            <a href="mailto:tchantha2004@gmail.com" class="hover:underline text-blue-400">tchantha2004@gmail.com</a>
          </div>
          <div class="flex items-center space-x-3">
            <span class="p-2 rounded-full bg-blue-400 text-gray-900">
              <i class="fas fa-phone"></i>
            </span>
            <p>0966463091</p>
          </div>
          <div class="flex items-center space-x-3">
            <span class="p-2 rounded-full bg-blue-400 text-gray-900">
              <i class="fab fa-telegram-plane"></i>
            </span>
            <a href="https://t.me/Touchh_Chantha" target="_blank" class="hover:underline text-blue-400">Telegram Account</a>
          </div>
          <div class="flex items-center space-x-3">
            <span class="p-2 rounded-full bg-blue-400 text-gray-900">
              <i class="fas fa-location-dot"></i>
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
  { name: 'Vue.js', icon: 'fab fa-vuejs' },
  { name: 'React.js', icon: 'fab fa-react' },
  { name: 'JavaScript', icon: 'fab fa-js' },
  { name: 'Tailwind CSS', icon: 'fas fa-wind' },
  { name: 'CSS 3', icon: 'fab fa-css3-alt' },
  { name: 'Bootstrap 5', icon: 'fab fa-bootstrap' },
  { name: 'Laravel', icon: 'fab fa-laravel' },
  { name: 'PHP', icon: 'fab fa-php' },
  { name: 'MySQL', icon: 'fas fa-database' },
  { name: 'Server', icon: 'fas fa-server' },
  { name: 'Github', icon: 'fab fa-github' },
]);
</script>