<script setup>
import CalculateForm from "@/components/CalculateForm.vue";
</script>

<template>
  <div class="layout">
    <CalculateForm />
  </div>
</template>

<style scoped>
.layout {
  @apply flex-1 p-2 w-full flex flex-col gap-3 items-center justify-start;
}
</style>
