<script setup>
import { defineProps } from "vue"
const props = defineProps(['title', 'description', 'image','price',"direction"])
import Button from "../ui/Button.vue"
</script>

<template>
    <div v-if="direction === 'left'"
        class="relative top-0 border px-8 rounded-[4rem] xl:rounded-[10rem] py-8 xl:py-16 2xl:py-24  border-gray-400 bg-white bg-opacity-10 backdrop-blur-sm ">
        <div class="absolute z-[40] md:-top-28 left-0  w-40 md:w-[25rem] xl:w-[35rem] 2xl:w-[37.5rem] lg:-top-48 object-contain object-center">
            <img class="w-full h-full " v-bind:src="image" alt="">
        </div>
        <div class="flex flex-col pl-32 md:pl-[20rem] xl:pl-[40rem] 2xl:pl-[50rem] w-full gap-2 lg:gap-5 relative z-[39] ">
            <p class="font-bold text-base lg:text-4xl">{{ props.title }}</p>
            <p class="font-light text-sm lg:text-xl">{{ props.description }}</p>
            <p class="font-bold text-base lg:text-4xl">${{ props.price }}</p>
            <div class="lg:mt-2">
                <Button>Explore</Button>
            </div>
        </div>
    </div>
    <div v-if="direction === 'right'"
        class="relative top-0 border px-8 rounded-[4rem] xl:rounded-[10rem] py-8 xl:py-16 2xl:py-24  border-gray-400 bg-white bg-opacity-10 backdrop-blur-sm ">
        
        <div class="flex flex-col  w-full gap-2 lg:gap-5 relative z-[39] pr-24 md:px-16 xl:px-36">
            <p class="font-bold text-base lg:text-4xl">{{ props.title }}</p>
            <p class="font-light text-sm lg:text-xl break-words w-auto md:w-8/12 lg:w-9/12 xl:w-8/12">{{ props.description }}</p>
            <p class="font-bold text-base lg:text-4xl">${{ props.price }}</p>
            <div class="lg:mt-2">
                <Button>Explore</Button>
            </div>
        </div>
        <div class="absolute z-[40] top-0 md:-top-28 right-0 md:-right-6 lg:-right-12 xl:right-0  w-40 md:w-[25rem] xl:w-[35rem] 2xl:w-[37.5rem] lg:-top-28 object-contain object-center">
            <img class="w-full h-full " v-bind:src="image" alt="">
        </div>
    </div>
</template>