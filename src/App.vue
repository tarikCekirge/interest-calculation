<script setup>
import LayoutView from "@/layouts/LayoutView.vue";
import ThemeSwitch from "@/components/ThemeSwitch.vue";
</script>

<template>
  <div class="app">
    <ThemeSwitch />
    <LayoutView />
  </div>
</template>
<style scoped>
.app {
  @apply w-full h-screen flex flex-col items-center justify-center;
}
</style>
