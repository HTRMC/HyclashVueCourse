<script setup lang="ts">
const items = [
  {
    id: 1,
    description: "The work on the infrastructure and architecture has been ongoing even before the release of Hytale. We've built a solid foundation, you won't need to wait long in order to play."
  },
  {
    id: 2,
    description: "The work on the infrastructure and release of Hytale. We've built a solid foundation, you won't need to wait long in order to play."
  },
  {
    id: 3,
    description: "The work on the infrastructure and architecture has been ongoing even before the release of Hytale. We've built a solid foundation, you won't need to wait long in order to play."
  }
]
</script>

<template>
  <section class="py-20 px-4 sm:px-6 lg:px-8">
    <div class="max-w-7xl mx-auto">
      <div class="text-center mb-12">
        <h2 class="text-3xl md:text-4xl font-bold text-white">TEMP</h2>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
        <div
          v-for="item in items"
          :key="item.id"
          class="space-y-4"
        >
          <!-- Image placeholder -->
          <div class="bg-gradient-to-br from-gray-800 to-gray-900 rounded-lg overflow-hidden border border-gray-700 aspect-video flex items-center justify-center">
            <div class="text-4xl">🎮</div>
          </div>

          <!-- Description -->
          <p class="text-gray-300 text-sm leading-relaxed">{{ item.description }}</p>
        </div>
      </div>
    </div>
  </section>
</template>
