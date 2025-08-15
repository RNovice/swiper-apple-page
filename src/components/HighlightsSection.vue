<template>
  <section class="section-highlights pt-24 pb-49">
    <div class="view-content">
      <h2 class="text-[26px] font-semibold pb-12">看這裡，畫重點。</h2>
    </div>
    <Swiper
      class="highlights-swiper pb-7.5!"
      :slides-per-view="1.2"
      :space-between="24"
      :centered-slides="true"
      :speed="900"
      :grab-cursor="true"
      @slideNextTransitionStart="handleSlide('next')"
      @slidePrevTransitionStart="handleSlide('prev')"
    >
      <SwiperSlide v-for="(item, i) in items" :key="i">
        <article
          :class="`highlight-card ${item.textButton ? 'child-end' : ''} `"
          :style="`background-image: url('${item.image}') `"
        >
          <p
            :class="`m-8 text-center font-semibold leading-[1.3] relative ${item.textStyle}`"
            v-html="item.content"
            :data-aos="currentAos"
            data-aos-duration="1000"
            :key="aosTrigger + i"
          ></p>
        </article>
      </SwiperSlide>
    </Swiper>
  </section>
</template>

<script setup>
import { Swiper, SwiperSlide } from 'swiper/vue'
import { ref, nextTick } from 'vue'
const aosTrigger = ref(0)
const currentAos = ref('fade-right')
const handleSlide = (direction) => {
  currentAos.value = direction === 'next' ? 'fade-left' : 'fade-right'

  nextTick(() => {
    aosTrigger.value += 1
  })
}
const items = [
  {
    content:
      '全新 Liquid Glass 設計<span class="absolute">，</span><br>好看、好愉悅、上手好熟悉<span class="absolute">。</span>',
    textButton: false,
    textStyle: '',
    image:
      'https://www.apple.com/tw/os/images/ios/highlights/liquid_glass__f595gw1ozwi2_small_2x.jpg',
  },
  {
    content:
      '<span class="text-nowrap">視覺智慧</span>讓你搜尋、提問，還能以 iPhone 螢幕內容進行更多操作<span class="absolute">。</span><span class="block text-[12px] mt-2.25 text-[#000000e0] font-normal">適用於特定語言</span>',
    textButton: false,
    textStyle: '',
    image:
      'https://www.apple.com/v/os/b/images/shared/highlights/visual_intelligence_startframe__eevpb4217oae_small_2x.jpg',
  },
  {
    content:
      '訊息 App 裡，聊天新背景更顯<span class="text-nowrap">個性，</span><br>有問題還可一起投票決定。',
    textButton: false,
    textStyle: 'text-start',
    image:
      'https://www.apple.com/v/os/b/images/ios/highlights/personalize__502614h12s2a_small_2x.jpg',
  },
  {
    content:
      '透過即時翻譯，在訊息 App、FaceTime 和電話中，不同語言<span class="text-nowrap">都能通。</span><span class="block text-[12px] mt-2.25 text-[#000000e0] font-normal">適用於特定語言</span>',
    textButton: false,
    textStyle: 'text-start',
    image:
      'https://www.apple.com/v/os/b/images/shared/highlights/live_translation__x2fac526k0im_small_2x.jpg',
  },
  {
    content:
      '全新篩選工具，幫你過濾<br>電話、FaceTime 和訊息<span class="absolute">，</span><br>避免各種干擾<span class="absolute">。</span>',
    textButton: true,
    textStyle: '',
    image:
      'https://www.apple.com/v/os/b/images/ios/highlights/screening_tools__14tk0zvttmqy_small_2x.jpg',
  },
  {
    content:
      'CarPlay 以即時動態讓你一覽更多<span class="text-nowrap">資訊<span class="absolute">，</span></span><br>還可快速點按<span class="nowrap">回應<span class="absolute">。</span></span>',
    textButton: false,
    textStyle: 'text-[#ffffffeb]',
    image: 'https://www.apple.com/v/os/b/images/ios/highlights/carplay__cfnmfvg0l0k2_small_2x.jpg',
  },
]
</script>
