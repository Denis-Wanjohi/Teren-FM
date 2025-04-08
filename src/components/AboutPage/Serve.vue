<script setup>
import Heading2 from '../Heading2.vue';
</script>
<template>
    <heading2 title="WE SERVE" mini_title=" We Serve" class="my-5"></heading2>
    <div class="w-10/12 mx-auto ">
        
        <div class="flex w-full h-[200px]">
            <div class="w-1/3 flex items-end justify-center"
                style="background-image: url('/images/AboutPage/office.png'); background-size: cover; object-fit: cover; object-position: center;">
                <p class="text-white bg-gradient-to-t cinzel lg:text-3xl text-xl from-black w-full text-center">Corporate offices</p>
            </div>
            <div class="w-1/3 flex items-end justify-center"
                style="background-image: url('/images/AboutPage/institution.png'); background-size: cover; object-fit: cover; object-position: center;">
                <p class="text-white bg-gradient-to-t cinzel lg:text-3xl text-xl from-black w-full text-center">Institutions</p>
            </div>
            <div class="w-1/3 flex items-end justify-center"
                style="background-image: url('/images/AboutPage/hotel.png'); background-size: cover; object-fit: cover; object-position: center;">
                <p class="text-white bg-gradient-to-t cinzel lg:text-3xl text-xl from-black w-full text-center">Hotels</p>
            </div>
        </div>
        <div class="flex w-full">
            <div class="w-1/2 h-[200px] flex items-end justify-center"
                style="background-image: url('/images/AboutPage/industries.png'); background-size: contain; object-fit: cover; object-position: center;">
                <p class="text-white bg-gradient-to-t cinzel lg:text-3xl text-xl from-black w-full text-center">Manufacturing Facilities</p>
            </div>
            <div class="w-1/2 h-[200px] flex items-end justify-center"
                style="background-image: url('/images/AboutPage/hospitals.png'); background-size: cover; object-fit: cover; object-position: center;">
                <p class="text-white bg-gradient-to-t cinzel lg:text-3xl text-xl from-black w-full text-center">Hospitals</p>
            </div>
        </div>
        <div class="flex w-full h-[200px]">
            <div class="w-1/3 flex items-end justify-center"
                style="background-image: url('/images/AboutPage/malls.png'); background-size: cover; object-fit: cover; object-position: center;">
                <p class="text-white bg-gradient-to-t cinzel lg:text-3xl text-xl from-black w-full text-center">Shopping malls</p>
            </div>
            <div class="w-1/3 flex items-end justify-center"
                style="background-image: url('/images/AboutPage/gvOffices.png'); background-size: cover; object-fit: cover; object-position: center;">
                <p class="text-white bg-gradient-to-t cinzel lg:text-3xl text-xl from-black w-full text-center">Government Offices</p>
            </div>
            <div class="w-1/3 flex items-end justify-center"
                style="background-image: url('/images/AboutPage/residentials.png'); background-size: cover; object-fit: cover; object-position: center;">
                <p class="text-white bg-gradient-to-t cinzel lg:text-3xl text-xl from-black w-full text-center">Residentials</p>
            </div>
        </div>
    </div>
</template>
<style>
img {
    object-fit: contain;
}
</style>