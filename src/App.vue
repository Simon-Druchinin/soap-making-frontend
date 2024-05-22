<script setup>
import Header from '@/layouts/Header.vue'

</script>

<style lang="scss">
@import "@/css/main.scss";
</style>


<template>
  <q-layout view="lHh lpr lFf" style="height: 100vh;" class="shadow-2 rounded-borders">
    <Header />
    <q-page-container class="bg-gradient">
      <RouterView />
    </q-page-container>
  </q-layout>
</template>
