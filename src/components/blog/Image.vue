<script setup lang="ts">
const props = defineProps<{
  legend: string;
}>()
</script>

<template>
  <div class="flex flex-col items-center justify-center gap-4 bg-white rounded-lg p-4 overflow-auto"
  >
    <slot></slot>
    <div class="text-center italic mt-2 mb-4" v-if="props.legend">
      {{ props.legend }}
    </div>
  </div>
</template>

<style scoped>

</style>