<script setup lang="ts">
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'
import HeroSection from './components/HeroSection.vue'
import WhatIsHyclash from './components/WhatIsHyclash.vue'
import TempSection from './components/TempSection.vue'
import BlogSection from './components/BlogSection.vue'
</script>

<template>
  <div class="min-h-screen flex flex-col">
    <Navbar />

    <main class="flex-1">
      <HeroSection />
      <WhatIsHyclash />
      <TempSection />
      <BlogSection />
    </main>

    <Footer />
  </div>
</template>

