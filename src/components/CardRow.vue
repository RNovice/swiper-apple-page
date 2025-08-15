<template>
  <Swiper slidesPerView="auto" spaceBetween="24" class="px-6.25! pt-2.5! pb-19!">
    <SwiperSlide v-for="(item, i) in slides" :key="i" class="w-65!">
      <img
        :src="item.image"
        :alt="rowName + '_img_' + i"
        class="rounded-[28px] h-[314px] bg-no-repeat bg-cover bg-center"
        data-aos="fade-up"
        data-aos-duration="1500"
      />
      <div
        class="pt-6 px-3.75 text-[12px]"
        data-aos="fade-up"
        data-aos-duration="1500"
        data-aos-delay="50"
      >
        <p v-html="item.content"></p>
      </div>
    </SwiperSlide>
  </Swiper>
</template>

<script setup>
import { Swiper, SwiperSlide } from 'swiper/vue'
defineProps({
  rowName: {
    type: String,
    default: '',
  },
  slides: {
    type: Array,
    default: () => [],
  },
})
</script>
