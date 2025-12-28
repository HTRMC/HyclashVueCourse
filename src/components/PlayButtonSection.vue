<script setup lang="ts">
</script>

<template>
  <section class="py-12 w-full">
    <div class="max-w-7xl mx-auto px-6 sm:px-8 lg:px-12">
      <div class="relative flex justify-center items-center">
        <!-- Fading line behind the button -->
        <div class="absolute inset-0 flex items-center">
          <div class="w-full h-0.5 bg-gradient-to-r from-transparent via-[rgb(95,97,97)] to-transparent"></div>
        </div>

        <!-- Button container -->
        <div class="relative bg-[#0e161f] border-2 border-[rgb(95,97,97)] rounded px-3 py-2 z-10">
          <!-- Play button -->
          <button class="bg-gradient-to-b from-[rgb(84,121,163)] to-[rgb(43,63,86)] hover:from-[rgb(94,131,173)] hover:to-[rgb(53,73,96)] text-white px-16 py-2 rounded border-2 border-[rgb(95,97,97)] text-xl font-semibold transition-all">
            PLAY
          </button>
        </div>
      </div>
    </div>
  </section>
</template>
