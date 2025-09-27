<script setup>
import { Icon } from '@iconify/vue'
</script>

<template>
  <section id="contacto" class="flex items-center justify-center py-5 md:py-15 bg-[#f9fafc]">
    <div class="max-w-7xl xl:max-w-[1400px] 2xl:max-w-[1600px] mx-auto px-4 lg:px-8 xl:px-12 2xl:px-16">
      <!-- Header Text -->
  <div class="text-center mb-12">
    <h2 class="text-4xl md:text-4xl font-bold text-gray-800 mb-6">Contáctanos</h2>
    <p class="text-lg md:text-xl text-gray-700 leading-relaxed">Have questions about our products or need custom designs? We'd love to hear from you!</p>
  </div>

  <!-- Contact Items -->
  <div class="flex flex-col md:flex-row justify-between items-center gap-8 md:gap-4 mb-12">
    
    <!-- Email Item -->
    <div class="text-center flex-1">
      <div class="flex justify-center mb-4">        
          <Icon icon="mdi:email" class="text-4xl text-[var(--primary)]"></Icon>
      </div>
      <h3 class="text-xl font-semibold text-gray-800 mb-2">Email</h3>
      <p class="text-gray-600">hello@alenna.com</p>
    </div>

    <!-- Phone Item -->
    <div class="text-center flex-1">
      <div class="flex justify-center mb-4">
          <Icon icon="mdi:phone" class="text-4xl text-[var(--primary)]"></Icon>
      </div>
      <h3 class="text-xl font-semibold text-gray-800 mb-2">Phone</h3>
      <p class="text-gray-600">+1 (555) 123-4567</p>
    </div>

    <!-- Hours Item -->
    <div class="text-center flex-1">
      <div class="flex justify-center mb-4">
          <Icon icon="mdi:schedule" class="text-4xl text-[var(--primary)]"></Icon>
      </div>
      <h3 class="text-xl font-semibold text-gray-800 mb-2">Hours</h3>
      <p class="text-gray-600">Mon-Fri 9AM-6PM</p>
    </div>

  </div>

  <!-- Send Message Button -->
  <div class="text-center">
    <a 
      href="https://wa.me/59174129131?text=Hi%20Alenna!%20I'm%20interested%20in%20your%203D%20printed%20cat%20gadgets.%20Could%20you%20tell%20me%20more%20about%20your%20products?"
      target="_blank"
      class="px-8 py-4 md:py-3 text-base lg:text-lg rounded-full bg-[var(--primary)] text-white font-semibold shadow-md hover:bg-[#713aed] transition inline-block"
    >
      Send message
    </a>
  </div>
    </div>
  </section>
</template>