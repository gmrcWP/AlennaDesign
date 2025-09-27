<script setup lang="ts">
import ProductsList from './ProductsList.vue';
import { RouterLink } from 'vue-router';
</script>

<template>
    <div id="productos" class="w-full mx-auto py-10 md:py-20 bg-[#f9fafc]">
        <div class="text-center mb-4 md:mb-10">
            <h2 class="text-2xl md:text-3xl font-[var(--montserrat)] font-bold text-gray-800">PRODUCTOS DESTACADOS</h2>
            <p class="mt-3 mx-1 text-md md:text-lg text-gray-800">Our most popular cat-themed 3D printed accessories</p>
        </div>

        <products-list :max-products="4" />

        <div class="mt-6 flex justify-center items-center">
            <RouterLink to="/productos" class="px-10 py-4 lg:py-3 font-[var(--montserrat)] text-base lg:text-lg rounded-full bg-[var(--primary)] text-white font-semibold shadow-md hover:bg-[#713aed] transition">
                Ver todos los productos
            </RouterLink>
        </div>
    </div>
</template>