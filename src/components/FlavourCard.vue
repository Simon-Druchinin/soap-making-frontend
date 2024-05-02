<script setup>
const props = defineProps(["form", "flavour"])
</script>

<template>
    <q-card
        @click="form.flavour = flavour.id"
        class="constructor__card"
        :class="{ 'selected': form.flavour === flavour.id }"
    >
        <q-card-section>
            <div class="column">
                <img class="constructor__card_img" :src="flavour.image" :alt="flavour.name" :key="flavour.id">
                <span class="text-center">{{  flavour.name }}</span>
            </div>
        </q-card-section>
    </q-card>
</template>
