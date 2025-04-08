<script setup>
import IconEmail from './icons/IconEmail.vue';
import IconPhone from './icons/IconPhone.vue';
import { Divider } from 'primevue';
</script>

<template>
    <div class="md:flex">
        <div class="md:w-1/3 text-center">
            <img src="/images/logo.png" class="mx-auto" alt="">
            <p class="px-10 lg:text-md text-sm">Teren Facilities management offers complete facilities solutions: from maintenance and operations to technology and sustainability, tailored to your needs</p>
        </div>
        <div class="flex md:w-2/3 justify-evenly font-bold text-xl items-center">
            <div class="leading-15">
                <router-link to="/">Home</router-link>
                <br>
                <router-link to="/about">About</router-link>
                <br>
                <router-link to="/services">Services</router-link>
              
            </div>
            <div class="leading-20">
                <div class="flex items-center">
                    <component :is="IconEmail"></component>
                    <p>info@terenfm.com</p>
                </div>
                <div class="flex items-center">
                    <component :is="IconPhone"></component>
                    <p>+254 702 841 930</p>
                </div>
            </div>
        </div>
    </div>
    <Divider></Divider>
    <p class="text-gray-400  text-center">@{{new Date().getFullYear()}}.TEREN FACILITIES MANAGAMENT LIMITED</p>
</template>