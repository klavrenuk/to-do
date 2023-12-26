<script setup lang="ts">
import AppHeader from "@/components/header/AppHeader.vue";

</script>

<template>
  <div class="app">
    <AppHeader />

    <main class="app_main" id="AppMain">
      <div class="container">
        <router-view/>
      </div>
    </main>
  </div>
</template>

<style lang="scss">
@import './assets/css/app.scss';
</style>
