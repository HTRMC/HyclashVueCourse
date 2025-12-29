<script setup lang="ts">
</script>

<template>
  <div class="fixed top-0 left-0 right-0 px-6 sm:px-8 lg:px-12 pt-12 z-50">
    <nav class="bg-[#0e161f]/50 backdrop-blur-[2px] max-w-7xl mx-auto relative rounded-xl">
      <!-- Top border with fade -->
      <div class="absolute top-0 left-0 right-0 h-px" style="background: linear-gradient(to right, #0e161f 0%, rgb(31, 41, 55) 2%, rgb(31, 41, 55) 98%, #0e161f 100%)"></div>
      <!-- Bottom border with fade -->
      <div class="absolute bottom-0 left-0 right-0 h-px" style="background: linear-gradient(to right, #0e161f 0%, rgb(31, 41, 55) 2%, rgb(31, 41, 55) 98%, #0e161f 100%)"></div>
      <div>
        <div class="flex items-center justify-between">
        <!-- Logo -->
        <div class="flex items-center gap-8">
          <div class="absolute top-1/2 -translate-y-1/2 left-0">
            <img src="/Logo.png" alt="HyClash Logo" class="h-24" />
          </div>
          <div class="w-20"></div>

          <!-- Navigation Links -->
          <div class="hidden md:flex items-center gap-6 font-['Cinzel']">
            <a href="#" class="text-gray-300 hover:text-white transition-colors font-semibold">Games</a>
            <a href="#" class="text-gray-300 hover:text-white transition-colors font-semibold">Leaderboards</a>
            <a href="#" class="text-gray-300 hover:text-white transition-colors font-semibold">Forums</a>
            <a href="#" class="text-gray-300 hover:text-white transition-colors font-semibold">Support</a>
            <a href="#" class="text-gray-300 hover:text-white transition-colors font-semibold">Store</a>
          </div>
        </div>

        <!-- Right side buttons -->
        <div class="flex items-center gap-4">
          <button class="text-gray-300 hover:text-white transition-colors font-['Cinzel'] font-semibold">Chaos</button>
          <button class="bg-gray-800 hover:bg-gray-700 text-white rounded-xl p-2 transition-colors">
            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z" />
            </svg>
          </button>
        </div>
        </div>
      </div>
    </nav>
  </div>
</template>
