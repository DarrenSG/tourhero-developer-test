<script setup>
import { ref } from 'vue'
import { Splide, SplideSlide } from '@splidejs/vue-splide'

defineProps({ day: Number, title: String, excerpt: String })

const showContent = ref(false)
</script>

<template>
  <div class="itinerary grid lg:grid-cols-[200px_1fr] gap-x-8">
    <Splide class="mb-auto" :options="{ rewind: true, pagination: false }">
      <SplideSlide
        ><img class="w-full rounded" :src="`https://picsum.photos/id/${day * 10}/300/200`"
      /></SplideSlide>
      <SplideSlide
        ><img class="w-full rounded" :src="`https://picsum.photos/id/${day + 40}/300/200`"
      /></SplideSlide>
    </Splide>
    <div class="flex flex-col gap-4">
      <div class="font-bold text-lg flex gap-4 mt-4 lg:mt-0">
        <div class="leading-tight text-blue-900 whitespace-nowrap">Day {{ day }}</div>
        <div class="leading-tight">{{ title }}</div>
      </div>
      <div class="leading-tight text-gray-500">{{ excerpt }}</div>
      <button
        class="text-cyan-700 mr-auto underline font-medium"
        v-if="!showContent"
        @click="showContent = true"
      >
        Show More
      </button>
      <div class="flex flex-col space-y-3" v-if="showContent"><slot /></div>
    </div>
  </div>
</template>

<style>
.itinerary .splide__arrow--prev,
.itinerary .splide__arrow--next {
  background-color: white;
  border: 1px solid #00000020;
  opacity: 1;
}

.itinerary .splide__arrow--prev {
  left: -15px;
}

.itinerary .splide__arrow--next {
  right: -15px;
}
</style>
