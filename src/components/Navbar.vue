<script setup>
import { ref } from 'vue';

let isMobileMenuOpen = ref(false);

const toggleMobileMenu = () => {
  isMobileMenuOpen.value = !isMobileMenuOpen.value;
}

const closeMobileMenu = () => {
  isMobileMenuOpen.value = false;
}
</script>

<template>
  <nav class="fixed top-0 left-0 right-0 bg-white/90 backdrop-blur-md shadow-lg z-50 transition-all duration-300">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between items-center py-4">
        <div class="text-xl font-[var(--montserrat)] font-bold text-gray-800">AlennaDesign</div>

        <!-- DESKTOP MENU -->
        <div class="hidden md:flex space-x-8">
          <a href="#inicio" class="nav-link text-gray-600 font-semibold hover:text-[var(--soft-primary)] transition-colors duration-200">Inicio</a>
          <a href="#productos" class="nav-link text-gray-600 font-semibold hover:text-[var(--soft-primary)] transition-colors duration-200">Productos</a>
          <a href="#acercade" class="nav-link text-gray-600 font-semibold hover:text-[var(--soft-primary)] transition-colors duration-200">Acerca de</a>
          <a href="#contacto" class="nav-link text-gray-600 font-semibold hover:text-[var(--soft-primary)] transition-colors duration-200">Contacto</a>
        </div>

        <!-- MOBILE HAMBURGER MENU -->
        <button @click="toggleMobileMenu()" class="md:hidden p-2 rounded-md hover:bg-gray-100 transition-color duration-200">
          <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
          </svg>
        </button>
      </div>

      <!-- MOBILE MENU -->
       <div class="md:hidden" v-if="isMobileMenuOpen">
          <div class="py-2 space-y-1">
            <a href="#inicio" @click="closeMobileMenu()" class="block px-3 py-2 text-gray-600 hover:text-blue-600 transition-colors duration-200">Inicio</a>
            <a href="#productos" @click="closeMobileMenu()" class="block px-3 py-2 text-gray-600 hover:text-blue-600 transition-colors duration-200">Productos</a>
            <a href="#acercade" @click="closeMobileMenu()" class="block px-3 py-2 text-gray-600 hover:text-blue-600 transition-colors duration-200">Acerca de</a>
            <a href="#contacto" @click="closeMobileMenu()" class="block px-3 py-2 text-gray-600 hover:text-blue-600 transition-colors duration-200">Contacto</a>
          </div>
       </div>
    </div>
  </nav>
</template>

<style scoped>
.nav-link {
  position: relative;
}

.nav-link::after {
  content: '';
  position: absolute;
  width: 0;
  height: 2px;
  bottom: -4px;
  left: 50%;
  background-color: var(--soft-primary);
  transition: all 0.3s ease;
}

.nav-link:hover::after {
  width: 100%;
  left: 0;
}
</style>
