<script setup>
import { defineProps } from 'vue';

</script>
<template>
    <h3 class="flex justify-center items-center text-white font-bold text-3xl text-center  md:text-6xl relative z-[5]">
        <img class="relative left-14 md:top-auto top-4" src="/titleLeft.png" alt="" srcset="">
        <span class="relative">
            <slot></slot>
        </span>
        <img class="relative right-14 md:top-auto -top-4" src="/titleRight.png" alt="" srcset="">
    </h3>
</template>