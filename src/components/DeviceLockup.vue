<template>
  <div class="relative h-[272px]">
    <div class="devices-lockup ios-device-lockup relative w-full h-full" role="img">
      <DeviceCard
        v-if="devices[2]"
        class="absolute left-1/2 top-1/2 z-[5] -translate-x-1/2 -translate-y-1/2 scale-100"
        :image="devices[2].src"
        :alt="devices[2].alt"
      />

      <DeviceCard
        v-if="devices[0]"
        class="absolute left-0 top-1/2 z-[2] -translate-y-1/2 sm:left-[16%]"
        :image="devices[0].src"
        :alt="devices[0].alt"
        :scale="0.725"
      />

      <DeviceCard
        v-if="devices[1]"
        class="absolute left-1/6 top-1/2 z-[3] -translate-y-1/2"
        :image="devices[1].src"
        :alt="devices[1].alt"
        :scale="0.875"
      />

      <DeviceCard
        v-if="devices[3]"
        class="absolute right-1/6 top-1/2 z-[3] -translate-y-1/2"
        :image="devices[3].src"
        :alt="devices[3].alt"
        :scale="0.875"
      />

      <DeviceCard
        v-if="devices[4]"
        class="absolute right-0 top-1/2 z-[2] -translate-y-1/2 sm:left-[84%]"
        :image="devices[4].src"
        :alt="devices[4].alt"
        :scale="0.725"
      />
    </div>
  </div>
</template>

<script setup>
import { defineProps } from 'vue'
import DeviceCard from './DeviceCard.vue'

defineProps({
  devices: {
    type: Array,
    default: () => [],
  },
})
</script>
