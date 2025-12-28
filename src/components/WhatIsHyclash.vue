<script setup lang="ts">
const features = [
  {
    id: 1,
    title: 'Lorem Ipsum is simply dummy text',
    description: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.'
  },
  {
    id: 2,
    title: 'Lorem Ipsum is simply dummy text',
    description: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.'
  },
  {
    id: 3,
    title: 'Lorem Ipsum is simply dummy text',
    description: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.'
  },
  {
    id: 4,
    title: 'Lorem Ipsum is simply dummy text',
    description: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.'
  }
]
</script>

<template>
  <section class="relative py-20 w-full overflow-hidden">
    <!-- Blurry background image -->
    <div class="absolute inset-0 z-0">
      <img
        src="/RunRun.jpg"
        alt="Background"
        class="w-full h-full object-cover blur-[2px] opacity-60"
      />
      <!-- Gradient overlays for vertical fade effect -->
      <div class="absolute inset-0 bg-gradient-to-b from-[#0e161f] via-transparent to-[#0e161f]"></div>
    </div>

    <div class="max-w-7xl mx-auto px-6 sm:px-8 lg:px-12 relative z-10">
      <div class="text-center mb-12">
        <h2 class="text-3xl md:text-4xl font-bold mb-4 font-['Cinzel'] bg-gradient-to-b from-[rgb(211,206,163)] to-[rgb(164,147,122)] bg-clip-text text-transparent">WHAT IS HYCLASH?</h2>
        <p class="text-gray-400 max-w-3xl mx-auto">
          Hyclash is a server (and game) experience unlike anything you've<br /> seen before! We've combined satisfying base building and resource<br /> management systems with the ability to queue into raids on other<br /> player's Strongholds! Much progression can also be found through<br /> expeditions (solo or co-op!) into mysterious dungeons. Well guarded<br /> and loot rich outposts. And an open world with countlress interesting<br /> characters and quests.
        </p>
      </div>

      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6">
        <div
          v-for="feature in features"
          :key="feature.id"
          class="bg-gray-900 rounded-lg overflow-hidden border border-gray-700 hover:border-blue-500 transition-colors"
        >
          <!-- Image placeholder -->
          <div class="aspect-video bg-gray-800 flex items-center justify-center">
          </div>

          <!-- Content -->
          <div class="p-4 space-y-3">
            <p class="text-gray-300 text-sm">{{ feature.description }}</p>
            <button class="w-full bg-gradient-to-b from-[rgb(84,121,163)] to-[rgb(43,63,86)] hover:from-[rgb(94,131,173)] hover:to-[rgb(53,73,96)] text-white py-2 rounded border-2 border-[rgb(95,97,97)] text-sm font-semibold font-['Cinzel'] transition-all">
              Learn More
            </button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
