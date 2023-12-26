<script setup lang="ts">
import AppLogo from "@/components/header/AppLogo.vue";
import AppHeaderController from "@/components/header/AppHeaderController.vue";
</script>

<template>
  <header class="app_header">
    <div class="container">
      <div class="flex justify-between items-center">
        <AppLogo />
        <AppHeaderController />
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
.app_header {
  padding: 1rem 0;
  background: #0066FF;
}
</style>
