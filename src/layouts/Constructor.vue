<style lang="scss">
@import "@/css/constructor.scss";
</style>

<script setup>
import { ref } from 'vue'

import cherryImage from "@/assets/cherry.png"
import raspberryImage from "@/assets/raspberry.png"
import strawberryImage from "@/assets/strawberry.png"
import appleImage from "@/assets/apple.png"
import mangoImage from "@/assets/mango.png"

const thumbStyle = {
    right: '4px',
    borderRadius: '5px',
    backgroundColor: '#ffad4a',
    height: '7px',
    opacity: 0.3,
}
const barStyle = {opacity: 0}

const form = ref({"flavour": null, "color": null})

const flavours = [
    {"id": 1, "name": "Вишня", "image": cherryImage},
    {"id": 2, "name": "Манго", "image": mangoImage},
    {"id": 3, "name": "Клубника", "image": strawberryImage},
    {"id": 4, "name": "Яблоко", "image": appleImage},
    {"id": 5, "name": "Малина", "image": raspberryImage},
]

const colors = [
    {"id": 3, "name": "Зелёный", "color": "linear-gradient(90deg, rgba(2,0,36,1) 0%, rgba(9,121,28,1) 35%, rgba(0,255,179,1) 100%)"},
    {"id": 1, "name": "Синий", "color": "linear-gradient(90deg, rgba(3,1,45,1) 0%, rgba(29,9,121,1) 35%, rgba(0,254,255,1) 100%)"},
    {"id": 2, "name": "Красный", "color": "linear-gradient(90deg, rgba(3,1,45,1) 0%, rgba(121,9,34,1) 35%, rgba(255,0,78,1) 100%)"},
    {"id": 4, "name": "Бирюзовый", "color": "linear-gradient(90deg, rgba(3,1,45,1) 0%, rgba(9,79,121,1) 35%, rgba(0,255,235,1) 100%)"},
    {"id": 5, "name": "Оранжевый", "color": "linear-gradient(90deg, rgba(3,1,45,1) 0%, rgba(121,78,9,1) 35%, rgba(255,132,0,1) 100%)"},
]

</script>


<template>
    <div class="column flex-center constructor__choices">
        <h5>Отдушка</h5>
        <q-scroll-area
            :thumb-style="thumbStyle"
            :bar-style="barStyle"
            style="height: 180px; width: 100vw; max-width: 80vw;"
        >
            <div class="row no-wrap flex-center constructor__flavours">
                <q-card
                    @click="form.flavour = flavour.id"
                    class="constructor__card"
                    :class="{ 'selected': form.flavour === flavour.id }"
                    v-for="flavour in flavours"
                >
                    <q-card-section>
                        <div class="column">
                            <img class="constructor__card_img" :src="flavour.image" :alt="flavour.name" :key="flavour.id">
                            <span class="text-center">{{  flavour.name  }}</span>
                        </div>
                    </q-card-section>
                </q-card>
            </div>
        </q-scroll-area>

        <h5>Цвет</h5>
        <q-scroll-area
            :thumb-style="thumbStyle"
            :bar-style="barStyle"
            style="height: 180px; width: 100vw; max-width: 80vw;"
        >
        <div class="row no-wrap flex-center constructor__colors">
            <q-card
                @click="form.color = color.id"
                class="constructor__card"
                :class="{ 'selected': form.color === color.id }"
                v-for="color in colors"
            >
                <q-card-section>
                    <div class="column">
                        <q-avatar size="70px" :style="`background: ${color.color}`"></q-avatar>
                        <span class="text-center q-pt-md">{{  color.name  }}</span>
                    </div>
                </q-card-section>
            </q-card>
        </div>
        </q-scroll-area>
    </div>
</template>
