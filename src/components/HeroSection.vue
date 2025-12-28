<script setup lang="ts">
</script>

<template>
  <section class="relative py-20 w-full">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-8 items-center">
        <!-- Left side - Welcome text -->
        <div class="space-y-6">
          <div>
            <p class="text-gray-400 text-sm uppercase tracking-wider mb-2">WELCOME TO</p>
            <h1 class="text-5xl md:text-6xl font-bold text-white">HYCLASH</h1>
          </div>
          <p class="text-gray-300 text-lg">
            An Open-world MMO RPG where you don't just live in a world - you own one.
          </p>
          <button class="bg-blue-600 hover:bg-blue-700 text-white px-6 py-3 rounded-md flex items-center gap-2 transition-colors">
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20">
              <path d="M10 12a2 2 0 100-4 2 2 0 000 4z"/>
              <path fill-rule="evenodd" d="M.458 10C1.732 5.943 5.522 3 10 3s8.268 2.943 9.542 7c-1.274 4.057-5.064 7-9.542 7S1.732 14.057.458 10zM14 10a4 4 0 11-8 0 4 4 0 018 0z" clip-rule="evenodd"/>
            </svg>
            <span>Discord Server</span>
          </button>
        </div>

        <!-- Right side - Promotional video/image -->
        <div class="relative">
          <div class="bg-gray-900 rounded-lg overflow-hidden border border-gray-700 aspect-video">
            <div class="w-full h-full flex items-center justify-center">
              <div class="text-center space-y-4">
                <div class="text-6xl">🎮</div>
                <p class="text-gray-400">Promotional Content Area</p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Play button -->
      <div class="mt-12 flex justify-center">
        <button class="bg-blue-600 hover:bg-blue-700 text-white px-12 py-3 rounded-md text-lg font-semibold transition-colors">
          PLAY
        </button>
      </div>
    </div>
  </section>
</template>
