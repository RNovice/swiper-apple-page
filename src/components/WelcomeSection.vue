<script setup lang="ts">
import DeviceLockup from './DeviceLockup.vue'
</script>

<template>
  <section
    class="section-welcome text-center bg-gradient-to-b from-[#ffffff] to-[#f5f5f7] pt-13.5 pb-24"
  >
    <div class="py-9">
      <div class="view-content">
        <div>
          <h1 class="header-eyebrow">iOS 26 預覽</h1>
          <h2 class="mt-1.5 text-[30px] font-semibold relative">
            面貌一新
            <span class="absolute">，</span>
            <br />上手更奇妙<span class="absolute">。</span>
          </h2>
        </div>
        <div class="mt-5">
          <p class="text-[#6e6e73]">秋季推出</p>
        </div>
      </div>
    </div>
    <DeviceLockup
      :devices="[
        {
          src: 'https://raw.githubusercontent.com/RNovice/swiper-apple-page/refs/heads/main/src/assets/images/welcome/welcome_ios_left2__b9y9q18mx9de_small_2x.png',
          alt: 'Left 2',
        },
        {
          src: 'https://raw.githubusercontent.com/RNovice/swiper-apple-page/refs/heads/main/src/assets/images/welcome/welcome_ios_left__vflvubgsgdem_small_2x.png',
          
          alt: 'Left 1',
        },
        {
          src: 'https://raw.githubusercontent.com/RNovice/swiper-apple-page/refs/heads/main/src/assets/images/welcome/welcome_ios_screen_startframe__f4qzub4umaum_small_2x.jpg',
          alt: 'Center',
        },
        {
          src: 'https://raw.githubusercontent.com/RNovice/swiper-apple-page/refs/heads/main/src/assets/images/welcome/welcome_ios_right__f6f221cowfe6_small_2x.png',
          alt: 'Right 1',
        },
        {
          src: 'https://raw.githubusercontent.com/RNovice/swiper-apple-page/refs/heads/main/src/assets/images/welcome/welcome_ios_right2__gganenisq7iy_small_2x.png',
          alt: 'Right 2',
        },
      ]"
    />
  </section>
</template>
