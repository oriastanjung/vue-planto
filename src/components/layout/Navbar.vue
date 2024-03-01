<script setup>
import { ref } from "vue"
const showMenu = ref(false)

</script>

<template>
    <header class="absolute w-full z-[100] px-2 py-4 lg:px-14 lg:py-16 text-white">
        <nav class="flex justify-between items-center">
            <h1 class="cursor-pointer text-3xl font-extrabold flex gap-2 items-center justify-center">
                <img class="w-11" src="/logo.png" alt="">Planto.
            </h1>
            <ul class="hidden lg:flex items-center flex-row gap-14 justify-center">
                <li class="cursor-pointer hover:underline text-2xl font-medium">Home</li>
                <li class="cursor-pointer hover:underline text-2xl font-medium">Plants Type</li>
                <li class="cursor-pointer hover:underline text-2xl font-medium">More</li>
                <li class="cursor-pointer hover:underline text-2xl font-medium">Contact</li>
            </ul>
            <div class="flex gap-5 lg:gap-14 items-center ">
                <div class="cursor-pointer">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                        stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round"
                            d="m21 21-5.197-5.197m0 0A7.5 7.5 0 1 0 5.196 5.196a7.5 7.5 0 0 0 10.607 10.607Z" />
                    </svg>

                </div>
                <div class="cursor-pointer">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                        stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round"
                            d="M15.75 10.5V6a3.75 3.75 0 1 0-7.5 0v4.5m11.356-1.993 1.263 12c.07.665-.45 1.243-1.119 1.243H4.25a1.125 1.125 0 0 1-1.12-1.243l1.264-12A1.125 1.125 0 0 1 5.513 7.5h12.974c.576 0 1.059.435 1.119 1.007ZM8.625 10.5a.375.375 0 1 1-.75 0 .375.375 0 0 1 .75 0Zm7.5 0a.375.375 0 1 1-.75 0 .375.375 0 0 1 .75 0Z" />
                    </svg>


                </div>
                <div class="cursor-pointer" @click="showMenu = !showMenu">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                        stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 9h16.5m-16.5 6.75h16.5" />
                    </svg>

                </div>
            </div>
            <div v-if="showMenu"
                class="lg:hidden h-screen w-full fixed z-[50] top-0 left-0 bg-white bg-opacity-15 backdrop-blur-md px-16 py-20">
                <div @click="showMenu = !showMenu" class="cursor-pointer flex justify-end absolute top-10 right-10">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-6 h-6">
                        <path fill-rule="evenodd"
                            d="M5.47 5.47a.75.75 0 0 1 1.06 0L12 10.94l5.47-5.47a.75.75 0 1 1 1.06 1.06L13.06 12l5.47 5.47a.75.75 0 1 1-1.06 1.06L12 13.06l-5.47 5.47a.75.75 0 0 1-1.06-1.06L10.94 12 5.47 6.53a.75.75 0 0 1 0-1.06Z"
                            clip-rule="evenodd" />
                    </svg>

                </div>
                <ul class="flex flex-col items-center gap-14 justify-center">
                    <li class="cursor-pointer hover:underline text-2xl font-medium">Home</li>
                    <li class="cursor-pointer hover:underline text-2xl font-medium">Plants Type</li>
                    <li class="cursor-pointer hover:underline text-2xl font-medium">More</li>
                    <li class="cursor-pointer hover:underline text-2xl font-medium">Contact</li>
                </ul>
            </div>
        </nav>
    </header>
</template>