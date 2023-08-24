<script setup>
import StarIcon from '@/components/icons/StarIcon.vue'

defineProps({ stars: Number })

const max = 5
</script>

<template>
  <div class="flex gap-1">
    <StarIcon v-for="i in stars" :key="i" class="w-4" color="#dc0909" />
    <StarIcon v-for="j in max - stars" :key="j" class="w-4" color="#aaaaaa" />
  </div>
</template>
