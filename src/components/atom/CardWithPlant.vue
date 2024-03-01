<script setup>
import { defineProps } from "vue"
const props = defineProps(['title', 'category', 'image'])
import Button from "../ui/Button.vue"
</script>

<template>
    <div
        class="relative top-0 border px-8 rounded-3xl w-56 h-[13rem] lg:w-96 lg:h-[30rem] border-gray-400 bg-white bg-opacity-10 backdrop-blur-sm">
        <div class="absolute z-[40] -top-28 left-5 lg:left-auto lg:-top-32 w-44 lg:w-80 object-contain object-center">
            <img class="w-full h-full " v-bind:src="image" alt="">
        </div>
        <div class="flex flex-col gap-2 lg:gap-5 relative top-16 lg:top-64">
            <p class="font-light text-sm lg:text-xl">{{ props.category }}</p>
            <p class="font-medium text-base lg:text-2xl">{{ props.title }}</p>
            <div class="lg:mt-2">
                <Button>Buy Now</Button>
            </div>
        </div>
    </div>
</template>