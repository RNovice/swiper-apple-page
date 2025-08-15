<script setup lang="ts">
import CardRow from './CardRow.vue'
</script>

<template>
  <section class="section-liquid-glass bg-[#f5f5f7]">
    <div
      class="bg-no-repeat bg-cover bg-bottom"
      style="
        background-image: url('https://www.apple.com/v/os/b/images/ios/liquid_glass/liquid_glass_hero__e4g9pjpws8ya_small_2x.jpg');
      "
    >
      <div class="view-content pt-12 pb-100 text-[#f5f5f7] text-center font-semibold">
        <h2 class="text-[19px] mt-[8.4px]">設計</h2>
        <p class="text-[38px]">
          全新元素<span class="absolute">，</span> <br />開啟愉悅新體驗<span class="absolute"
            >。</span
          >
        </p>
      </div>
    </div>
    <div class="view-content">
      <p class="py-12 mb-[8.4px] text-[#6e6e73] text-[19px] font-semibold tracking-[-0.5px]">
        全新的 Liquid Glass 設計，不僅外觀<span class="text-nowrap">好看，</span
        >使用愉悅，而且一上手就好熟悉。在所有 app
        和各個裝置上，它都帶來更一致的使用體驗，讓一切操控有如行雲流水般
        <span class="text-nowrap">流暢。</span>
      </p>
    </div>
    <CardRow
      rowName="liquid-glass"
      :slides="[
        {
          content: `<h3 class='inline font-semibold'>新設計，新意滿點。</h3><p class='inline'>Liquid&nbsp;Glass 結合玻璃的光學品質與流暢靈動的特質，為你的「鎖定畫面」、「主畫面」、「控制中心」和各款 app，帶來滿滿表達力的全新設計。</p>`,
          image:
            'https://www.apple.com/v/os/b/images/ios/liquid_glass/design__51h6pg9xusii_small_2x.jpg',
        },
        {
          content: `<h3 class='inline font-semibold'>更鮮活靈動的鎖定畫面。</h3><p class='inline'>時間顯示會根據背景圖片和通知動態調整，確保照片主角始終是焦點。當你稍微轉動 iPhone 時，照片更會以全新的 3D 效果鮮活<span class='text-nowrap'>呈現。</span></p>`,
          image:
            'https://www.apple.com/v/os/b/images/shared/liquid_glass/lock_screen__bd82spxl9k9u_small_2x.jpg',
        },
        {
          content: `<h3 class='inline font-semibold'>App 圖像，通透大更新。</h3><p class='inline'>經過更新的淺色與深色外觀、全新可調成不同色調或耀眼透明的圖像樣式，都任你挑選。</p>`,
          image:
            'https://www.apple.com/v/os/b/images/shared/liquid_glass/app_icons__ghno6awtphe2_small_2x.jpg',
        },
        {
          content: `<h3 class='inline font-semibold'>動態控制項目。</h3><p class='inline'>各款 app 中的 Liquid&nbsp;Glass 控制項目，會折射並映現周圍內容，變化流暢自然，讓你的專注力聚焦於內容本身。</p>`,
          image:
            'https://www.apple.com/v/os/b/images/shared/liquid_glass/dynamic_controls__ezqkwhge3vsm_small_2x.jpg',
        },
        {
          content: `<h3 class='inline font-semibold'>全系統，風格一致。</h3>
									<p class='inline'>Liquid&nbsp;Glass 賞心悅目的體驗，遍及各個 app 和裝置，方便你整天隨時切換，更輕鬆地使用 Apple 各個產品。</p>`,
          image:
            'https://www.apple.com/v/os/b/images/ios/liquid_glass/refreshed_apps__cz8url2r74mu_small_2x.jpg',
        },
      ]"
    />
  </section>
</template>
