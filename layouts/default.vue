<template>
  <div>
    <NuxtLoadingIndicator />

    <slot></slot>
    <AppFooter />
  </div>
</template>
<script setup>
import { onMounted } from "vue";

onMounted(() => {
  window.addEventListener("load", () => {
    // Hide the loading indicator when the page is fully loaded
    NuxtLoadingIndicator.finish();
  });
});
</script>
