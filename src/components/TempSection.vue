<script setup lang="ts">
const items = [
  {
    id: 1,
    image: '/CorruptedGolem.jpg',
    alt: 'CorruptedGolem',
    description: "The work on the infrastructure and architecture has been ongoing even before the release of Hytale. We've built a solid foundation, you won't need to wait long in order to play."
  },
  {
    id: 2,
    image: '/Friends.jpg',
    alt: 'Friends',
    description: "The work on the infrastructure and release of Hytale. We've built a solid foundation, you won't need to wait long in order to play."
  },
  {
    id: 3,
    image: '/Explore.jpg',
    alt: 'Explore',
    description: "The work on the infrastructure and architecture has been ongoing even before the release of Hytale. We've built a solid foundation, you won't need to wait long in order to play."
  }
]
</script>

<template>
  <section class="relative py-20 w-full">
    <div class="max-w-7xl mx-auto px-6 sm:px-8 lg:px-12 relative z-10">
      <div class="text-center mb-12">
        <h2 class="text-3xl md:text-4xl font-bold mb-4 font-['Cinzel'] bg-gradient-to-b from-[rgb(211,206,163)] to-[rgb(164,147,122)] bg-clip-text text-transparent">TEMP</h2>
        <div class="w-full h-0.5 bg-gradient-to-r from-transparent via-[rgb(95,97,97)] to-transparent"></div>
      </div>

      <div class="space-y-12">
        <div
          v-for="(item, index) in items"
          :key="item.id"
          class="grid grid-cols-1 md:grid-cols-2 gap-8 items-center"
        >
          <!-- Image -->
          <div
            class="bg-gray-900 rounded-4xl overflow-hidden border border-gray-700 aspect-video relative"
            :class="index % 2 === 1 ? 'md:order-2' : ''"
          >
            <img :src="item.image" :alt="item.alt" class="w-full h-full object-cover" />
            <!-- Gradient overlay -->
            <div
              class="absolute inset-0 pointer-events-none"
              :class="index % 2 === 1 ? 'bg-gradient-to-r from-[rgb(9,13,14)] from-0% via-transparent via-20% to-transparent' : 'bg-gradient-to-l from-[rgb(9,13,14)] from-0% via-transparent via-20% to-transparent'"
            ></div>
          </div>

          <!-- Description -->
          <p
            class="text-white font-semibold text-sm leading-relaxed"
            :class="index % 2 === 1 ? 'md:order-1' : ''"
          >
            {{ item.description }}
          </p>
        </div>
      </div>
    </div>
  </section>
</template>
