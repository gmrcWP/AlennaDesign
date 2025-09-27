<script setup>
import { Icon } from '@iconify/vue';
</script>

<template>
  <footer class="bg-[#202938] py-12">
    <div class="max-w-7xl xl:max-w-[1400px] 2xl:max-w-[1600px] mx-auto px-4 lg:px-8 xl:px-12 2xl:px-16">
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8 lg:gap-12">
        
        <div class="space-y-4">
          <h3 class="text-2xl font-bold text-white">Alenna</h3>
          <p class="text-[var(--gray)] leading-relaxed">Creating purr-fect 3D printed gadgets for your feline friends.</p>
          <div class="flex space-x-4 pt-2">
            <a href="#" class="text-[var(--gray)]">
              <Icon icon="mdi:facebook" class="text-2xl text-white hover:text-[var(--primary)] transition-colors duration-300"></Icon>
            </a>
            <a href="#" class="text-[var(--gray)]">
              <Icon icon="ic:baseline-tiktok" class="text-2xl text-white hover:text-[var(--primary)] transition-colors duration-300"></Icon>
            </a>
            <a href="#" class="text-[var(--gray)]">
              <Icon icon="mdi:instagram" class="text-2xl text-white hover:text-[var(--primary)] transition-colors duration-300"></Icon>
            </a>
          </div>
        </div>


        <div class="space-y-4">
          <h3 class="text-xl font-semibold text-white">Quick Links</h3>
          <ul class="space-y-3">
            <li><a href="#" class="text-[var(--gray)] hover:text-white transition-colors duration-300">Home</a></li>
            <li><a href="#" class="text-[var(--gray)] hover:text-white transition-colors duration-300">Products</a></li>
            <li><a href="#" class="text-[var(--gray)] hover:text-white transition-colors duration-300">About</a></li>
            <li><a href="#" class="text-[var(--gray)] hover:text-white transition-colors duration-300">Contact</a></li>
          </ul>
        </div>

        <div class="space-y-4">
          <h3 class="text-xl font-semibold text-white">Categories</h3>
          <ul class="space-y-3">
            <li><a href="#" class="text-[var(--gray)] hover:text-white transition-colors duration-300">Feeders</a></li>
            <li><a href="#" class="text-[var(--gray)] hover:text-white transition-colors duration-300">Toys</a></li>
            <li><a href="#" class="text-[var(--gray)] hover:text-white transition-colors duration-300">Furniture</a></li>
          </ul>
        </div>

      </div>
    </div>
  </footer> 
</template>