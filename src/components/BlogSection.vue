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
    <div class="max-w-7xl mx-auto px-6 sm:px-8 lg:px-12">
      <div class="text-center mb-12">
        <h2 class="text-3xl md:text-4xl font-bold text-white mb-4">BLOG</h2>
        <div class="w-full h-0.5 bg-gradient-to-r from-transparent via-[rgb(95,97,97)] to-transparent"></div>
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
        <button class="bg-linear-to-b from-[rgb(46,66,92)] to-[rgb(28,45,66)] hover:from-[rgb(56,76,102)] hover:to-[rgb(38,55,76)] text-white px-5 py-1 rounded-xl border-2 border-[rgb(95,97,97)] font-semibold transition-all">
          READ MORE
        </button>
      </div>
    </div>
  </section>
</template>
