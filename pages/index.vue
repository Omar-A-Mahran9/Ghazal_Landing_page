<template>
  <div style="direction: rtl">
    <div class="hero_section"></div>
    <div class="main_section container">
      <AppNav class="container mt-5 mb-5" />
      <Herosection style="margin-top: 40px" />
    </div>
    <secsection />
    <sec-section />
    <third-section />
    <fifth-section style="margin-top: 50px; margin-bottom: 100px" />
    <last-section />
  </div>
</template>
<script setup>
const { locale } = useI18n();
</script>
<style>
.hero_section {
  position: absolute;
  width: 100%; /* Set the width as needed */
  height: 890px;
  background: linear-gradient(to right, #2d9596 0%, #3cadae 100%);
  clip-path: ellipse(130% 80% at 35% 0%);
}
.main_section {
  height: 800px;
}
@media screen and (max-width: 959px) {
  .hero_section {
    position: absolute;
    width: 100%; /* Set the width as needed */
    height: 600px;
    background: linear-gradient(to right, #2d9596 0%, #3cadae 100%);
    clip-path: polygon(0% 0%, 100% 0%, 100% 100%, 0% 100%);
  }
  .main_section {
    height: 650px;
  }
}
</style>
