<script setup>
import CardRow from './CardRow.vue'
</script>

<template>
  <section class="section-intelligence bg-[#f5f5f7] pt-24">
    <div class="view-content">
      <div class="pb-12 font-semibold">
        <h2 class="text-[19px]" data-aos="fade-up" data-aos-duration="1000">Apple Intelligence</h2>
        <p class="text-[38px]" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="50">
          天天好用，<br />輕鬆幫忙。
        </p>
        <p
          class="text-[19px] text-[#6e6e73]"
          data-aos="fade-up"
          data-aos-duration="1000"
          data-aos-delay="50"
        >
          Apple Intelligence
          已整合到更多地方，幫助你在不同語言中溝通無礙，打造更多個人專屬影像，並使用更強大的捷徑<span
            class="text-nowrap"
            >功能。</span
          >
        </p>
      </div>
    </div>
    <CardRow
      :slides="[
        {
          content: `<h3 class='inline font-semibold'>即時翻譯。</h3><p class='inline'>自動為你翻譯「訊息」中的<span class='text-nowrap'>文字，</span>在 FaceTime 通話時顯示即時翻譯字幕，還能在「電話」app 中提供通話的語音<span class='text-nowrap'>翻譯。</span></p>`,
          image:
            'https://www.apple.com/v/os/b/images/shared/apple_intelligence/live_translation__x2fac526k0im_small_2x.jpg',
        },
        {
          content: `<h3 class='inline font-semibold'>視覺智慧，幫你做更多。</h3><p class='inline'>它以 Apple&nbsp;Intelligence 技術打造，讓你可在最常用的 app 上盡情搜尋，將行程加入行事曆，還能提問題，並以螢幕內容就能做到更多事。</p>`,
          image:
            'https://www.apple.com/v/os/b/images/shared/apple_intelligence/content_screen_endframe__dxlrxyvnyfo2_large.jpg',
        },
        {
          content: `<h3 class='inline font-semibold'>用影像表達自我，有更多玩法。</h3><p class='inline'>利用表情符號加上描述，就能創作全新表情。在「影像樂園」中，還有更多 ChatGPT 風格等你去探索。透過 Genmoji 與「影像樂園」，以親朋好友的影像為靈感時，擁有更多掌控進行<span class='text-nowrap'>創作。</span></p>`,
          image:
            'https://www.apple.com/v/os/b/images/shared/apple_intelligence/genmoji__b2htoaj2to76_small_2x.jpg',
        },
        {
          content: `<h3 class='inline font-semibold'>加速你的工作流程。</h3><p class='inline'>「捷徑」中的智慧操作可以摘要文字、建立影像，或直接調用 Apple&nbsp;Intelligence 模型，將得到的回應輸入至捷徑。</p>`,
          image:
            'https://www.apple.com/v/os/b/images/shared/apple_intelligence/icon_ask_model__d1tqjy3fi3ma_small_2x.jpg',
        },
      ]"
    />
  </section>
</template>
