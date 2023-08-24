<script setup>
import { SplideSlide } from '@splidejs/vue-splide'
import PlayButton from '@/components/PlayButton.vue'

defineProps({ src: String })
</script>

<template>
  <SplideSlide>
    <div class="relative grid place-items-center">
      <img :src="src" class="rounded-lg" />
      <PlayButton class="absolute w-[100px] z-10" />
    </div>
  </SplideSlide>
</template>
