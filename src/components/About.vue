<script setup></script>

<template>
  <section id="acercade" class="flex items-center justify-center py-5 md:py-15">
    <div class="max-w-7xl xl:max-w-[1400px] 2xl:max-w-[1600px] mx-auto px-4 lg:px-8 xl:px-12 2xl:px-16">
      <div class="flex flex-col-reverse md:flex-row items-center gap-8 lg:gap-12 xl:gap-16 2xl:gap-18">
        
        <div class="flex-1 max-w-xl lg:max-w-2xl xl:max-w-3xl text-left mx-auto">
          <div class="text-left md:mb-10">
            <h2 class="text-2xl md:text-3xl font-[var(--montserrat)] font-bold text-gray-800">ABOUT ALENNA</h2>
            <p class="mt-3 text-md md:mt-8 md:text-lg text-gray-900">We're passionate cat lovers who believe every feline deserves the best. Using cutting-edge 3D printing technology, we create innovative, safe, and fun gadgets that enhance the lives of cats and their owners.</p>
            <p class="mt-3 text-md md:mt-8 md:text-lg text-gray-900">Our products are designed with both functionality and aesthetics in mind, ensuring they fit seamlessly into your home while providing endless entertainment for your furry friends.</p>
          </div>

          
          <div class="mt-4 lg:mt-10 flex flex-col md:flex-row gap-3 lg:gap-10 sm:justify-start justify-center">
            <div>
              <h1 class="flex items-center justify-center text-3xl font-bold font-[var(--montserrat)] text-[var(--primary)]">500+</h1>
              <p class="flex items-center justify-center text-gray-700 text-md">Happy Cats</p>
            </div>
            <div>
              <h1 class="flex items-center justify-center text-3xl font-bold font-[var(--montserrat)] text-[var(--primary)]">50+</h1>
              <p class="flex items-center justify-center text-gray-700 text-md">Unique products</p>
            </div>
            <div>
              <h1 class="flex items-center justify-center text-3xl font-bold font-[var(--montserrat)] text-[var(--primary)]">99%</h1>
              <p class="flex items-center justify-center text-gray-700 text-md">Satisfaction Rate</p>
            </div>           
          </div>
        </div>

        <div class="flex-1 hidden md:flex flex items-center justify-center mt-10 md:mt-0">
          <img src="@/assets/about.jpg" loading="lazy" class="w-[360px] h-[280px] md:w-[300px] md:h-[220px] lg:w-[400px] lg:h-[300px] xl:w-[500px] xl:h-[380px] 2xl:w-[630px] 2xl:h-[440px] rounded-2xl shadow-lg" />
        </div>

      </div>
    </div>
  </section>
</template>
