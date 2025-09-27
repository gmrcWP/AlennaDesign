<script setup>
import ProductsList from '@/components/ProductsList.vue';
</script>

<template>
   <div class="w-full mx-auto py-10 md:py-20 bg-[#f9fafc]">
      <products-list :max-products="1" />       
    </div>
</template>