<script setup>
const props = defineProps(["form", "color"])
</script>

<template>
    <q-card
        @click="form.color = color.id"
        class="constructor__card"
        :class="{ 'selected': form.color === color.id }"
    >
        <q-card-section>
            <div class="column">
                <q-avatar size="70px" :style="`background: ${color.color}`"></q-avatar>
                <span class="text-center q-pt-md">{{  color.name  }}</span>
            </div>
        </q-card-section>
    </q-card>
</template>