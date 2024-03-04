<script setup>
import { defineProps } from "vue"
const props = defineProps(['title', 'description','price', 'image'])
import Button from "../ui/Button.vue"

</script>

<template>
    <div
        class="mt-16 md:mt-28 relative top-0 border px-8 rounded-3xl h-56 md:h-[17rem] xl:h-[27rem] border-gray-400 bg-white bg-opacity-10 backdrop-blur-sm">
        <div class="absolute z-[40] -top-20 md:-top-28 left-0 lg:-left-3 xl:-left-10 2xl:left-[3rem] lg:-top-40 md:w-80 lg:w-72 xl:w-[30rem] object-contain object-center">
            <img class="w-full h-full " v-bind:src="image" alt="">
        </div>
        <div class="flex flex-col gap-4  xl:gap-8 relative top-10  md:top-32 lg:top-16 xl:top-52">
            <p class="font-light text-base lg:text-2xl">{{ props.title }}</p>
            <p class="font-extralight text-sm lg:text-xl">{{ props.description }}</p>
            <div class="flex justify-between items-center">
                <p class="font-light text-base lg:text-2xl">${{ props.price }}</p>
                <button class="px-2 py-1 border rounded-md">
                    <v-icon name="hi-shopping-bag" fill="white"/>
                </button>
            </div>
            <!-- <div class="lg:mt-2">
                <Button>Buy Now</Button>
            </div> -->
        </div>
    </div>
</template>