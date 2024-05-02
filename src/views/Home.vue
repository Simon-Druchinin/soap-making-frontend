<style lang="scss">
@import "@/css/greeting.scss";
@import "@/css/features.scss";
@import "@/css/about.scss";
</style>

<script setup>
import Constructor from '@/layouts/Constructor.vue'
</script>


<template>
    <section class="row greeting__section" id="greeting">
        <div class="col greeting__left">
            <h5 class="greeting__title-above">Добро пожаловать <span class="text-primary">к Кате</span></h5>
            <h3 class="greeting__title-main">Где <span class="text-primary">мыло</span> превращается в искусство.</h3> 
            <p class="greeting__text">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                Laudantium, nulla aut iure libero maiores culpa, recusandae minus provident, id odit quos.
                Vero eum inventore consequuntur vitae a harum ex accusamus.
                Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                Laudantium, nulla aut iure libero maiores culpa, recusandae minus provident, id odit quos.
                Vero eum inventore consequuntur vitae a harum ex accusamus.
            </p>
            <q-btn class="greeting__btn" href="#constructor" color="primary" rounded no-caps>Заказать</q-btn>
            <div class="row greeting__achieves">
                <div class="column greeting__achieves-text" style="height: 150px">
                    <span class="text-bold">5000 +</span>
                    <span class="text-bold text-grey-5">Customer</span>
                </div>
                <div class="column greeting__achieves-text q-ml-md" style="height: 150px">
                    <span class="text-bold">10 000</span>
                    <span class="text-bold text-grey-5">Delivery</span>
                </div>
                <div class="column greeting__achieves-text q-ml-md" style="height: 150px">
                    <span class="text-bold">100 000</span>
                    <span class="text-bold text-grey-5">Business</span>
                </div>
            </div>
        </div>

        <div class="col greeting__right">
            <div class="greeting__circle"></div>
            <div class="greeting__circle"></div>
            <div class="greeting__circle"></div>
            <div class="greeting__circle"></div>
            <div class="greeting__circle"></div>
            <div class="greeting__img">
                <div class="greeting__square"></div>
                <div class="greeting__square"></div>
                <img src="@/assets/soap500x500.jpg" alt="soap500x500">
            </div>
        </div>
    </section>
    <section class="row features__section">
        <div class="column flex-center">
            <span class="text-bold text-primary">FEATURES</span>
            <h4 class="text-bold text-center">Варим мыло с любовью</h4>
            <div class="row features__items">
                <div class="column features__item">
                    <q-avatar color="grey-3" size="80px">
                        <img class="q-pa-sm" src="@/assets/logo.svg" alt="logo">
                    </q-avatar>
                    <div class="text-bold">Природные ингридиенты</div>
                    <p class="text-center">
                        Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                        Repellat sunt, deleniti repellendus incidunt suscipit optio nemo
                        exercitationem quasi neque ad quaerat similique dolorum odit pariatur facere voluptate tenetur aliquid ipsa!
                    </p>
                </div>
                <div class="column features__item">
                    <q-avatar color="grey-3" size="80px">
                        <img class="q-pa-sm" src="@/assets/logo.svg" alt="logo">
                    </q-avatar>
                    <div class="text-bold">Природные ингридиенты</div>
                    <p class="text-center">
                        Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                        Repellat sunt, deleniti repellendus incidunt suscipit optio nemo
                        exercitationem quasi neque ad quaerat similique dolorum odit pariatur facere voluptate tenetur aliquid ipsa!
                    </p>
                </div>
                <div class="column features__item">
                    <q-avatar color="grey-3" size="80px">
                        <img class="q-pa-sm" src="@/assets/logo.svg" alt="logo">
                    </q-avatar>
                    <div class="text-bold">Природные ингридиенты</div>
                    <p class="text-center">
                        Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                        Repellat sunt, deleniti repellendus incidunt suscipit optio nemo
                        exercitationem quasi neque ad quaerat similique dolorum odit pariatur facere voluptate tenetur aliquid ipsa!
                    </p>
                </div>
            </div>
        </div>
    </section>
    <section class="row flex-center about__section" id="about">
        <div class="column flex-center q-mt-lg">
            <span class="text-bold text-primary">FEATURES</span>
            <h4 class="text-bold">О нас</h4>
            <p class="text-center about__text">
                Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                Repellat sunt, deleniti repellendus incidunt suscipit optio nemo
                exercitationem quasi neque ad quaerat similique dolorum odit pariatur facere voluptate tenetur aliquid ipsa!
            </p>
        </div>
    </section>
    <section class="constructor__section" id="constructor">
        <Constructor />
    </section>
</template>