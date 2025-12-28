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
  <section class="py-20 w-full">
    <div class="max-w-7xl mx-auto px-6 sm:px-8 lg:px-12">
      <div class="text-center mb-12">
        <h2 class="text-3xl md:text-4xl font-bold text-white mb-4">WHAT IS HYCLASH?</h2>
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
            <button class="w-full bg-blue-600 hover:bg-blue-700 text-white py-2 rounded-md text-sm font-semibold transition-colors">
              Learn More
            </button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
