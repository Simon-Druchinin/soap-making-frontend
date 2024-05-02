<script setup>
import Header from '@/layouts/Header.vue'
import Footer from '@/layouts/Footer.vue'

</script>

<style lang="scss">
@import "@/css/main.scss";
</style>


<template>
  <q-layout view="lHh lpr lFf" style="height: 100vh;overflow-y:scroll;-webkit-overflow-scrolling:touch" class="shadow-2 rounded-borders">
    <Header />
    <q-page-container class="bg-gradient">
      <RouterView />
      <q-page-scroller position="bottom-right" :scroll-offset="150" :offset="[18, 18]">
        <q-btn fab icon="keyboard_arrow_up" color="primary" />
      </q-page-scroller>
    </q-page-container>
    <!-- <Footer /> -->
  </q-layout>
</template>
