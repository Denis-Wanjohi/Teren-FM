<script setup lang="ts">
import router from '@/router';
import { Button, Drawer } from 'primevue';
import { ref } from 'vue';
const isMenu = ref(false)
</script>

<template>
    <div class="flex justify-between h-[60px] bg-blue-400 open-sans py-1 sm:px-10 pl-10 pr-3">
        <img src="/images/logo.png" @click="router.push('/')" alt="">
        <div class="sm:block hidden w-1/2" >
            <div class="flex justify-around items-center font-sans text-md ">
                <p @click="router.push('/')" class="hover:cursor-pointer hover:bg-blue-300 px-2 py-2 rounded">HOME</p>
                <p @click="router.push('/about')" class="hover:cursor-pointer hover:bg-blue-300 px-2 py-2 rounded">ABOUT
                </p>
                <p @click="router.push('/services')" class="hover:cursor-pointer hover:bg-blue-300 px-2 py-2 rounded">
                    SERVICES</p>
            </div>
        </div>
        <div class="sm:hidden block">
            <Button class="h-fit my-auto" severity="info" @click="isMenu = true">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                <rect width="24" height="24" fill="none" />
                <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2">
                    <path d="M5 5L19 19M5 19L19 5">
                        <animate fill="freeze" attributeName="d" dur="0.36s"
                            values="M5 5L19 19M5 19L19 5;M5 5L19 5M5 19L19 19" />
                    </path>
                    <path d="M12 12H12" opacity="0">
                        <animate fill="freeze" attributeName="d" begin="0.18s" dur="0.36s"
                            values="M12 12H12;M5 12H19" />
                        <set fill="freeze" attributeName="opacity" begin="0.18s" to="1" />
                    </path>
                </g>
            </svg>
        </Button>
        </div>
    </div>
    <Drawer :visible="isMenu" :show-close-icon="false">
        <p class="text-end" @click="isMenu = false">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                <rect width="24" height="24" fill="none" />
                <mask id="lineMdCloseCircleFilled0">
                    <g fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="2">
                        <path fill="#fff" fill-opacity="0" stroke-dasharray="64" stroke-dashoffset="64"
                            d="M12 3c4.97 0 9 4.03 9 9c0 4.97 -4.03 9 -9 9c-4.97 0 -9 -4.03 -9 -9c0 -4.97 4.03 -9 9 -9Z">
                            <animate fill="freeze" attributeName="fill-opacity" begin="0.78s" dur="0.65s"
                                values="0;1" />
                            <animate fill="freeze" attributeName="stroke-dashoffset" dur="0.78s" values="64;0" />
                        </path>
                        <path stroke="#000" stroke-dasharray="8" stroke-dashoffset="8"
                            d="M12 12l4 4M12 12l-4 -4M12 12l-4 4M12 12l4 -4">
                            <animate fill="freeze" attributeName="stroke-dashoffset" begin="1.43s" dur="0.26s"
                                values="8;0" />
                        </path>
                    </g>
                </mask>
                <rect width="24" height="24" fill="currentColor" mask="url(#lineMdCloseCircleFilled0)" />
            </svg>
        </p>
        <div>
            <p class="text-center font-bold text-xl">TEREN FACILITIES MANAGEMENT</p>
            <div class="text-center">
                <div class="leading-15" @click="isMenu = false">
                    <router-link to="/">Home</router-link>
                    <br>
                    <router-link to="/about">About</router-link>
                    <br>
                    <router-link to="/services">Services</router-link>
                </div>
            </div>
        </div>
    </Drawer>
</template>

<style>
.open-sans {
    font-family: "Open Sans", sans-serif;
    font-optical-sizing: auto;
    font-weight: 600;
    font-style: normal;
    font-variation-settings:
        "wdth" 100;
}
</style>