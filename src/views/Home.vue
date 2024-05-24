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
            <h5 class="greeting__title-above">Добро пожаловать <span class="text-primary">в мыльную оранжерею,</span></h5>
            <h3 class="greeting__title-main">Где <span class="text-primary">цветы</span> превращаются в искусство.</h3> 
            <p class="greeting__text">
                Мимолетность красоты, хрупкость жизни и цениность каждого мгновения все это несет в себе очаровательный и пьянящий пион. 
                Действительно, ароматные и нежные лепестки пионов держатся всего несколько дней, напоминая нам, что жизнь слишком коротка, и мы должны наслаждаться каждым моментом
                 и ценить красоту вокруг нас. Наша мыловарня может помочь Вам по-новому выразить свои чувства окружающим с помощью 
                 хрупкого и сказочного мыла-цветка, который сможет радовать не один день.

            </p>
            <q-btn class="greeting__btn" href="#constructor" color="primary" rounded no-caps>Создать свой цветок</q-btn>
            <div class="row greeting__achieves">
                <div class="column greeting__achieves-text" style="height: 150px">
                    <span class="text-bold">5000 +</span>
                    <span class="text-bold text-grey-5">Клиентов</span>
                </div>
                <div class="column greeting__achieves-text q-ml-md" style="height: 150px">
                    <span class="text-bold">10 000</span>
                    <span class="text-bold text-grey-5">Доставок</span>
                </div>
                <div class="column greeting__achieves-text q-ml-md" style="height: 150px">
                    <span class="text-bold">1000</span>
                    <span class="text-bold text-grey-5">Позиций</span>
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
                    <div class="text-h6"><u>Природные ингридиенты</u></div>
                    <p class="text-center text-italic">
                        Основа произведена по современной рецептуре с использованием высококачественного сырья. 
                        Не содержит Лаурилсульфат натрия, то есть она SLS Free.
                        Вместо этого, довольно агрессивного компонента, она содержит более мягкие, щадящие кожу.
                       
                    </p>
                </div>
                <div class="column features__item">
                    <q-avatar color="grey-3" size="80px">
                        <img class="q-pa-sm" src="@/assets/logo.svg" alt="logo">
                    </q-avatar>
                    <div class="text-h6"><u>Неповторимый аромат</u></div>
                    <p class="text-center text-italic">
                        Разнообразная коллекция оттушек, которые придадут Ваши цветам приятные фруктовые, цветочные, ягодные, травяные ароматы. 
                        В основе присутствует фиксатор аромата, который усиливает и продлевает действие аромата отдушек.
                    </p>
                </div>
                <div class="column features__item">
                    <q-avatar color="grey-3" size="80px">
                        <img class="q-pa-sm" src="@/assets/logo.svg" alt="logo">
                    </q-avatar>
                    <div class="text-h6 text-underline"><u>Оригинальность</u></div>
                    <p class="text-center text-italic">
                        Одним из важных пунктов языка цветов является цвет. 
                        Создайте  полностью индивидуальную работу, благодаря нашим ярким и насыщенным оттенкам.
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
                Наша мыловарная-оранжерея "Мылыч" только начала свой путь, 
                но мы с большим удовольствием продвигаем ее и дарим Вам незабываемые чувста и эмоции.
                 Скоро в нашей оранжереи будут новые цветы: шелковые розы и благоухающие нарциссы.
            </p>
        </div>
    </section>
    <section class="constructor__section" id="constructor">
        <Constructor />
    </section>
</template>