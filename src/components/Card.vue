<script setup>
  defineProps({
  title: String,
  description: String,
})
</script>

<template>
  <div class="bg-white rounded-lg p-4 h-40 max-w-96 border border-black">
    <h2 class="text-2xl font-semibold mb-10">{{ title }}</h2>
      <p class="text-gray-600 max-w-96">{{ description }}</p>
  </div>
</template>

<style scoped>

</style>