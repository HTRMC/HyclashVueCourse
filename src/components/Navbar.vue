<script setup lang="ts">
</script>

<style scoped>
.nav-link {
  color: white;
  transition: all 0.3s ease;
}

.nav-link:hover {
  background: linear-gradient(to bottom, rgb(211, 206, 163), rgb(164, 147, 122));
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
}
</style>

<template>
  <div class="fixed top-0 left-0 right-0 px-6 sm:px-8 lg:px-12 pt-12 z-50">
    <nav class="bg-[#0e161f]/45 backdrop-blur-[2px] max-w-7xl mx-auto relative">
      <!-- Top border with fade -->
      <div class="absolute top-0 left-0 right-0 h-px" style="background: linear-gradient(to right, transparent 0%, rgb(95, 97, 97) 5%, rgb(95, 97, 97) 95%, transparent 100%)"></div>
      <!-- Bottom border with fade -->
      <div class="absolute bottom-0 left-0 right-0 h-px" style="background: linear-gradient(to right, transparent 0%, rgb(95, 97, 97) 5%, rgb(95, 97, 97) 95%, transparent 100%)"></div>

      <div class="py-px relative z-10">
        <div class="flex items-center justify-between">
        <!-- Logo -->
        <div class="flex items-center gap-8">
          <div class="absolute top-1/2 -translate-y-1/2 left-0">
            <img src="/Logo.png" alt="HyClash Logo" class="h-24" />
          </div>
          <div class="w-20"></div>

          <!-- Navigation Links -->
          <div class="hidden md:flex items-center gap-2 font-['Cinzel']">
            <a href="#" class="nav-link font-semibold">Games</a>
            <div class="h-4 w-0.5 bg-[rgb(95,97,97)]"></div>
            <a href="#" class="nav-link font-semibold">Leaderboards</a>
            <div class="h-4 w-0.5 bg-[rgb(95,97,97)]"></div>
            <a href="#" class="nav-link font-semibold">Forums</a>
            <div class="h-4 w-0.5 bg-[rgb(95,97,97)]"></div>
            <a href="#" class="nav-link font-semibold">Support</a>
            <div class="h-4 w-0.5 bg-[rgb(95,97,97)]"></div>
            <a href="#" class="nav-link font-semibold">Store</a>
          </div>
        </div>

        <!-- Right side buttons -->
        <div class="flex items-center gap-4">
          <button class="nav-link font-['Cinzel'] font-semibold">Chaos</button>
          <button class="bg-gray-800 hover:bg-gray-700 text-white rounded-2xl p-2.5 border-2 border-[rgb(95,97,97)] transition-colors">
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
