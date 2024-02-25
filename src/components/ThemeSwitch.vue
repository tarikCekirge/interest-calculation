<script setup>
import { useDark, useToggle } from "@vueuse/core";

const isDark = useDark();
const toggleDark = useToggle(isDark);
</script>

<template>
  <div class="theme-switch">
    <button class="theme-btn" @click="toggleDark()">
      <span :class="isDark ? 'translate-x-6' : 'translate-x-1'" class="inline-block h-4 w-4 transform rounded-full bg-gray-800 dark:bg-slate-100"></span>
    </button>
  </div>
</template>

<style scoped>
.theme-switch {
  @apply ml-auto p-2;
}
.theme-btn {
  @apply h-6 w-11 flex items-center justify-start rounded-full bg-slate-100 dark:bg-slate-500;
}
</style>
