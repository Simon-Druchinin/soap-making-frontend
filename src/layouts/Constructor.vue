<style lang="scss">
@import "@/css/constructor.scss";
</style>

<script setup>
import cherryImage from "@/assets/cherry.png"
import { ref } from 'vue'

const form = ref({"flavour": null})

const flavours = [
    {"id": 1, "name": "Вишня", "image": cherryImage},
    {"id": 2, "name": "Вишня", "image": cherryImage},
    {"id": 3, "name": "Вишня", "image": cherryImage},
    {"id": 4, "name": "Вишня", "image": cherryImage},
    {"id": 5, "name": "Вишня", "image": cherryImage},
]
console.log(form.value)
</script>


<template>
    <div class="column flex-center">
        <h5>Отдушка</h5>
        <div class="row flex-center constructor__flavours">
            <q-card
                @click="form.flavour = flavour.id"
                class="constructor__card"
                :class="{ 'selected': form.flavour === flavour.id }"
                v-for="flavour in flavours"
            >
                <q-card-section>
                    <div class="column">
                        <img style="width: 50px" :src="flavour.image" :alt="flavour.name" :key="flavour.id">
                        <span class="text-center">{{  flavour.name  }}</span>
                    </div>
                </q-card-section>
            </q-card>
        </div>
    </div>
</template>
