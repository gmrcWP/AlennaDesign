<script setup></script>

<template>
  <nav class="fixed top-0 left-0 right-0 bg-white/90 backdrop-blur-md shadow-sm z-50 transition-all duration-300">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between items-center py-4">
        <div class="text-xl font-[var(--main-font)] font-bold text-gray-800">AlennaDesign</div>

        <div class="hidden md:flex space-x-8">
          <a href="#inicio" class="nav-link text-gray-600 font-semibold hover:text-[var(--soft-primary)] transition-colors duration-200">Inicio</a>
          <a href="#productos" class="nav-link text-gray-600 font-semibold hover:text-[var(--soft-primary)] transition-colors duration-200">Productos</a>
          <a href="#acercade" class="nav-link text-gray-600 font-semibold hover:text-[var(--soft-primary)] transition-colors duration-200">Acerca de</a>
          <a href="#contacto" class="nav-link text-gray-600 font-semibold hover:text-[var(--soft-primary)] transition-colors duration-200">Contacto</a>
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
