<style lang="scss">
@import "@/css/header.scss";
</style>

<template>
    <q-header class="transparent text-primary" ref="headRef">
        <q-toolbar class="q-mt-md q-mb-md">
        <q-avatar>
            <img src="@/assets/logo.svg" alt="logo">
        </q-avatar>
        <q-toolbar-title class="text-h5">Мылыч</q-toolbar-title>
        
        <nav>
            <RouterLink to="/">Главная</RouterLink>
            <a href="#about">О нас</a>
        </nav>
        </q-toolbar>
    </q-header>

</template>
