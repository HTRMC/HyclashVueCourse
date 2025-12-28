<script setup lang="ts">
const blogPosts = [
  {
    id: 1,
    title: 'HYCLASH BLOG',
    description: "The work on the infrastructure and architecture has been ongoing even before the release of Hytale. We've built a solid foundation, you won't need to wait long in order to play."
  },
  {
    id: 2,
    title: 'HYCLASH BLOG',
    description: "The work on the infrastructure and architecture has been ongoing even before the release of Hytale. We've built a solid foundation, you won't need to wait long in order to play."
  },
  {
    id: 3,
    title: 'HYCLASH BLOG',
    description: "The work on the infrastructure and architecture has been ongoing even before the release of Hytale. We've built a solid foundation, you won't need to wait long in order to play."
  }
]
</script>

<template>
  <section class="py-20 w-full">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-12">
        <h2 class="text-3xl md:text-4xl font-bold text-white">BLOG</h2>
      </div>

      <div class="space-y-6 max-w-4xl mx-auto">
        <div
          v-for="post in blogPosts"
          :key="post.id"
          class="bg-gray-900 rounded-lg overflow-hidden border border-gray-700 hover:border-blue-500 transition-colors"
        >
          <div class="grid grid-cols-1 md:grid-cols-3 gap-4 p-4">
            <!-- Image -->
            <div class="aspect-video md:aspect-square bg-gray-800 rounded-lg flex items-center justify-center">
            </div>

            <!-- Content -->
            <div class="md:col-span-2 flex flex-col justify-center space-y-3">
              <h3 class="text-white font-semibold text-lg">{{ post.title }}</h3>
              <p class="text-gray-400 text-sm">{{ post.description }}</p>
            </div>
          </div>
        </div>
      </div>

      <div class="mt-12 flex justify-center">
        <button class="bg-blue-600 hover:bg-blue-700 text-white px-8 py-3 rounded-md font-semibold transition-colors">
          READ MORE
        </button>
      </div>
    </div>
  </section>
</template>
