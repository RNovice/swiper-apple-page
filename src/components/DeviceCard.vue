<template>
  <div class="device-card aspect-[9/19] h-full" :style="{ transform: `scale(${scale})` }">
    <div class="h-full w-full rounded-[2.2rem]">
      <img class="h-full w-full rounded-[1.9rem]" :src="image" :alt="alt" draggable="false" />
    </div>
  </div>
</template>

<script setup>
defineProps({
  image: { type: String, required: true },
  alt: { type: String, default: '' },
  scale: { type: Number, default: 1 },
})
</script>
