<script setup lang="ts">
import { ref } from 'vue';
import CardProductVue from '../atom/CardProduct.vue';
import SectionTitle from '../atom/SectionTitle.vue';

type PlantType = {
    title: string;
    description : string
    price : number
    image: string
}

const dataPlants = ref<PlantType[]>([
    {
        title :"Calathea plant",
        description : "Lorem ipsum dolor sit amet, consectetur adipiscing elit",
        price : 359,
        image : "/plant1.png"
    },
    {
        title :"Calathea plant",
        description : "Lorem ipsum dolor sit amet, consectetur adipiscing elit",
        price : 359,
        image : "/plant2.png"
    },
    {
        title :"Calathea plant",
        description : "Lorem ipsum dolor sit amet, consectetur adipiscing elit",
        price : 359,
        image : "/plant3.png"
    },
    {
        title :"Calathea plant",
        description : "Lorem ipsum dolor sit amet, consectetur adipiscing elit",
        price : 359,
        image : "/plant4.png"
    },
    {
        title :"Calathea plant",
        description : "Lorem ipsum dolor sit amet, consectetur adipiscing elit",
        price : 359,
        image : "/plant5.png"
    },
    {
        title :"Calathea plant",
        description : "Lorem ipsum dolor sit amet, consectetur adipiscing elit",
        price : 359,
        image : "/plant6.png"
    },
])
</script>
<template>
    <section class="relative top-48 md:top-32 xl:top-32 2xl:top-[45rem]  px-6 py-3 z-10 lg:px-14 lg:py-16 w-full">
        <SectionTitle>Our Top Selling</SectionTitle>
        <div class="mt-16 md:mt-16 grid grid-cols-2 lg:grid-cols-3 gap-4 md:gap-10 ">
            <CardProductVue v-for="(item,idx) of dataPlants" :image="item.image" :title="item.title" :description="item.description" :price="item.price"/>
        </div>
    </section>
</template>