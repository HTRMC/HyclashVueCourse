<script setup lang="ts">
interface Props {
  src: string
  alt?: string
  blur?: string
  opacity?: string
  translateY?: string
}

const props = withDefaults(defineProps<Props>(), {
  alt: 'Background',
  blur: 'blur-[2px]',
  opacity: 'opacity-60',
  translateY: '0%'
})
</script>

<template>
  <div class="absolute inset-0 z-0">
    <div class="relative w-full h-full" :style="{ transform: `translateY(${translateY})` }">
      <img
        :src="src"
        :alt="alt"
        :class="`w-full h-full object-cover ${blur} ${opacity}`"
      />
      <!-- Gradient overlays for vertical fade effect -->
      <div class="absolute -inset-1 bg-gradient-to-b from-[#0e161f] from-0% via-[#0e161f]/70 via-20% to-transparent to-40%"></div>
      <div class="absolute -inset-1 bg-gradient-to-t from-[#0e161f] from-0% via-[#0e161f]/70 via-20% to-transparent to-40%"></div>
    </div>
  </div>
</template>
