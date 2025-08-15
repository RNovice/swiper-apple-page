<script setup>
import HighlightsSection from './components/HighlightsSection.vue'
import LiquidGlassSection from './components/LiquidGlassSection.vue'
import WelcomeSection from './components/WelcomeSection.vue'
import 'swiper/css'
</script>

<template>
  <div class="globalheader">
    <nav class="globalheader"></nav>
    <div id="globalnav-placeholder" class="globalnav-placeholder"></div>
  </div>
  <nav class="os-localnav"></nav>
  <main>
    <WelcomeSection />
    <HighlightsSection />
    <LiquidGlassSection />
  </main>
</template>
