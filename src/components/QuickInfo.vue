<script setup>
defineProps({ icon: String, label: String, text: String })
</script>

<template>
  <div class="flex flex-col gap-2">
    <span class="material-symbols-outlined text-cyan-600 leading-none">{{ icon }}</span>
    <div class="text-xs text-gray-400 leading-none uppercase">{{ label }}</div>
    <div class="font-medium leading-none">{{ text }}</div>
  </div>
</template>
