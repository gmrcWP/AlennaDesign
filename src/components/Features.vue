<script setup>
import { Icon } from '@iconify/vue'
</script>

<template>
  <div class="xl:max-w-[1550px] mx-auto px-6 py-16 grid grid-cols-1 md:grid-cols-3 gap-5 md:gap-12 text-center">
    
    <div class="md:max-w-lg mx-auto">
      <div class="flex items-center justify-center mb-4">
        <div class="w-18 h-18 flex items-center justify-center rounded-full bg-[#f3edff]">
          <Icon icon="mdi:cube-outline" class="text-[var(--primary)] text-3xl" />
        </div>
      </div>
      <h3 class="text-lg font-semibold text-gray-800 md:mb-5">3D Printed Quality</h3>
      <p class="mt-2 text-gray-800">
        Each product is carefully crafted using premium PLA materials for durability and precision.
      </p>
    </div>

    
    <div class="md:max-w-lg mx-auto">
      <div class="flex items-center justify-center mb-4">
        <div class="w-18 h-18 flex items-center justify-center rounded-full bg-[#fef5e6]">
          <Icon icon="mdi:heart" class="text-[#f39c10] text-3xl" />
        </div>
      </div>
      <h3 class="text-lg font-semibold text-gray-800 md:mb-5">Cat-Themed Designs</h3>
      <p class="mt-2 text-gray-800">
        Adorable feline-inspired designs that bring joy to your everyday essentials.
      </p>
    </div>

    
    <div class="md:max-w-lg mx-auto">
      <div class="flex items-center justify-center mb-4">
        <div class="w-18 h-18 flex items-center justify-center rounded-full bg-[#feebf7]">
          <Icon icon="mdi:truck-fast" class="text-[#e54a95] text-3xl" />
        </div>
      </div>
      <h3 class="text-lg font-semibold text-gray-800 md:mb-5">Fast Shipping</h3>
      <p class="mt-2 text-gray-800">
        Quick delivery to get your cat gadgets to you as soon as possible.
      </p>
    </div>
  </div>
</template>