<script setup>
import HighlightsSection from './components/HighlightsSection.vue'
import WelcomeSection from './components/WelcomeSection.vue'
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
  </main>
</template>
