<script setup lang="ts">
</script>

<template>
  <nav class="bg-[#0a0f16] border-b border-gray-800">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-16">
        <!-- Logo -->
        <div class="flex items-center gap-8">
          <div class="flex items-center gap-2">
            <img src="@/assets/logo.svg" alt="HyClash Logo" class="w-8 h-8" />
            <span class="text-white font-bold text-lg">HyClash</span>
          </div>

          <!-- Navigation Links -->
          <div class="hidden md:flex items-center gap-6">
            <a href="#" class="text-gray-300 hover:text-white transition-colors">Games</a>
            <a href="#" class="text-gray-300 hover:text-white transition-colors">Leaderboards</a>
            <a href="#" class="text-gray-300 hover:text-white transition-colors">Forums</a>
            <a href="#" class="text-gray-300 hover:text-white transition-colors">Support</a>
            <a href="#" class="text-gray-300 hover:text-white transition-colors">Store</a>
          </div>
        </div>

        <!-- Right side buttons -->
        <div class="flex items-center gap-4">
          <button class="text-gray-300 hover:text-white transition-colors">Clans</button>
          <button class="bg-gray-800 hover:bg-gray-700 text-white rounded-full p-2 transition-colors">
            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z" />
            </svg>
          </button>
        </div>
      </div>
    </div>
  </nav>
</template>
