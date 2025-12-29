<script setup lang="ts">
import BackgroundImage from './BackgroundImage.vue'
</script>

<template>
  <section class="relative pt-64 pb-20 w-full overflow-hidden">
    <BackgroundImage src="/hero-bg.jpg" opacity="opacity-90" :fade-top="false" />

    <!-- Horizontal fade overlays -->
    <div class="absolute inset-0 bg-linear-to-r from-[#0e161f] via-transparent to-[#0e161f] z-1"></div>

    <div class="max-w-7xl mx-auto px-6 sm:px-8 lg:px-12 relative z-10">
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-8 items-center">
        <!-- Left side - Welcome text -->
        <div class="space-y-6">
          <div class="inline-block">
            <div class="text-center">
              <p class="text-2xl font-semibold uppercase tracking-wider font-['Cinzel'] bg-linear-to-b from-[rgb(211,206,163)] to-[rgb(164,147,122)] bg-clip-text text-transparent">WELCOME TO</p>
              <h1 class="text-5xl md:text-6xl font-bold bg-linear-to-b from-[rgb(211,206,163)] to-[rgb(164,147,122)] bg-clip-text text-transparent">HYCLASH</h1>
            </div>
          </div>
          <p class="text-white text-lg font-semibold">
            An Open-world MMO RPG where you<br />
            don't just live in a world - you run one.
          </p>
          <a
            href="https://discord.gg/c9BFeKmcxq"
            rel="noopener noreferrer"
            target="_blank"
            class="rounded-md font-medium inline-flex items-center transition-colors px-3 py-2 text-base gap-2 ring-1 ring-inset ring-gray-700 text-white bg-gray-800 hover:bg-gray-700 active:bg-gray-700 focus:outline-none focus-visible:ring-2 focus-visible:ring-blue-500"
          >
            <svg class="shrink-0 w-6 h-6" aria-hidden="true" viewBox="0 0 24 24" fill="currentColor">
              <path d="M20.317 4.37a19.791 19.791 0 0 0-4.885-1.515a.074.074 0 0 0-.079.037c-.21.375-.444.864-.608 1.25a18.27 18.27 0 0 0-5.487 0a12.64 12.64 0 0 0-.617-1.25a.077.077 0 0 0-.079-.037A19.736 19.736 0 0 0 3.677 4.37a.07.07 0 0 0-.032.027C.533 9.046-.32 13.58.099 18.057a.082.082 0 0 0 .031.057a19.9 19.9 0 0 0 5.993 3.03a.078.078 0 0 0 .084-.028a14.09 14.09 0 0 0 1.226-1.994a.076.076 0 0 0-.041-.106a13.107 13.107 0 0 1-1.872-.892a.077.077 0 0 1-.008-.128a10.2 10.2 0 0 0 .372-.292a.074.074 0 0 1 .077-.01c3.928 1.793 8.18 1.793 12.062 0a.074.074 0 0 1 .078.01c.12.098.246.198.373.292a.077.077 0 0 1-.006.127a12.299 12.299 0 0 1-1.873.892a.077.077 0 0 0-.041.107c.36.698.772 1.362 1.225 1.993a.076.076 0 0 0 .084.028a19.839 19.839 0 0 0 6.002-3.03a.077.077 0 0 0 .032-.054c.5-5.177-.838-9.674-3.549-13.66a.061.061 0 0 0-.031-.03zM8.02 15.33c-1.183 0-2.157-1.085-2.157-2.419c0-1.333.956-2.419 2.157-2.419c1.21 0 2.176 1.096 2.157 2.42c0 1.333-.956 2.418-2.157 2.418zm7.975 0c-1.183 0-2.157-1.085-2.157-2.419c0-1.333.955-2.419 2.157-2.419c1.21 0 2.176 1.096 2.157 2.42c0 1.333-.946 2.418-2.157 2.418z"/>
            </svg>
            <span class="truncate">Join our Discord</span>
          </a>
        </div>

        <!-- Right side - Promotional video/image -->
        <div class="relative">
          <div class="bg-gray-900 rounded-lg overflow-hidden border border-gray-700 aspect-video">
            <iframe
              class="w-full h-full"
              src="https://www.youtube.com/embed/s3rI4mhIveA"
              title="YouTube video player"
              frameborder="0"
              allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
              allowfullscreen
            ></iframe>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
