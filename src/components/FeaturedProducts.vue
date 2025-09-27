<script setup lang="ts">
import type { Product } from '@/types/product.type';

const products: Product[] =[
    {
        id: 1,
        isBestSeller: true,
        image: "/products/product1.jpg",
        name: "Cat Phone Holder",
        description: "Adorable sitting cat design that holds your phone securely",
        price: 24.99,
    },
    {
        id: 2,
        isBestSeller: false,
        image: "/products/product2.jpeg",
        name: "Cat Pin Collection",
        description: "Set of 6 cute cat pins in various poses and colors",
        price: 18.99,
    },
    {
        id: 3,
        isBestSeller: false,
        image: "/products/product3.png",
        name: "Cat Cup Holder",
        description: "Functional cat-shaped coaster and cup holder",
        price: 16.99,
    },
    {
        id: 4,
        isBestSeller: false,
        image: "/products/product4.PNG",
        name: "Cat Desk Organizer",
        description: "Multi-compartment organizer with cat design",
        price: 32.99,
    },  
];

</script>

<template>
  <div class="w-full mx-auto py-10 md:py-20 bg-[#f9fafc]">
    <div class="text-center mb-4 md:mb-10">
      <h2 class="text-2xl md:text-3xl font-[var(--montserrat)] font-bold text-gray-800">PRODUCTOS DESTACADOS</h2>
      <p class="mt-3 mx-1 text-md md:text-lg text-gray-800">Our most popular cat-themed 3D printed accessories</p>
    </div>

    <div class="xl:max-w-[1550px] mx-auto">
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-3 md:gap-0">
            
            
            <div 
                v-for="product in products" 
                :key="product.id" 
                class="bg-white rounded-2xl shadow-lg hover:shadow-xl overflow-hidden relative mx-10 md:m-4 group"
            >
                
                <div 
                    v-if="product.isBestSeller" 
                    class="absolute top-4 right-4 z-10"
                >
                  <span class="bg-[var(--soft-primary)] text-white px-3 py-1 rounded-full text-sm font-medium">Más Vendido</span>
                </div>
                
               
                <div class="h-64 bg-gray-100 flex items-center justify-center  overflow-hidden">
                  <img 
                    :src="product.image" 
                    loading="lazy" 
                    class="w-full h-full object-cover transition-transform duration-300 group-hover:scale-105" 
                  />
                </div>
                
                <div class="p-6">
                    <h3 class="text-lg font-[var(--montserrat)] font-bold text-gray-800 mb-2">{{ product.name }}</h3>
                    <p class="text-gray-600 text-md mb-4">{{ product.description }}</p>
                    
                    <div class="flex items-center justify-between">
                        <span class="text-2xl font-bold text-[var(--primary)]">BOB {{ product.price }}</span>
                        <button class="bg-[var(--primary)] hover:bg-violet-600 text-white px-4 py-2 rounded-full transition-colors">
                            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 3h2l.4 2M7 13h10l4-8H5.4m0 0L7 13m0 0l-1.1 5.4M7 13v4a2 2 0 002 2h6a2 2 0 002-2v-4"></path>
                            </svg>
                        </button>
                    </div>
                </div>
            </div>

        </div>
    </div>

    <div class="mt-6 flex justify-center items-center">
        <a href="#"class="px-10 py-4 lg:py-3 font-[var(--montserrat)] text-base lg:text-lg rounded-full bg-[var(--primary)] text-white font-semibold shadow-md hover:bg-[#713aed] transition">
            Ver todos los productos
        </a>
    </div>
  </div>
</template>