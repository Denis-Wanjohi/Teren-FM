<script setup>
import router from '@/router';
import { Button } from 'primevue';
import Services from '@/components/HomePage/Services.vue';
import Value from '@/components/HomePage/Value.vue';
import CTA from '@/components/CTA.vue';
import Heading from '@/components/Heading.vue';
const whyData = [
  {
    label: 'Expertise & Experience',
    desc: 'Our skilled team delivers effective FM solutions with deep industry knowledge.'
  },
  {
    label: 'Cost-Effective Operations',
    desc: 'We optimize your budget to deliver value and reduce operational costs.'
  },
  {
    label: 'Sustainability Focus',
    desc: 'Committed to green, eco-friendly solutions for a sustainable future.'
  },
  {
    label: 'End-to-End Solutions',
    desc: 'We provide comprehensive hard and soft FM services for all your needs'
  },
  {
    label: '24/7 Support & Emergency Response',
    desc: 'We provide round-the-clock support and emergency response to ensure your business continuity.'
  }
]
</script>

<template>
  
  <main>
    <!-- HERO SECTION -->
    <div class="md:flex items-center px-10 min:h-[60vh] ">
      <img src="/images/hero.png" class="lg:w-1/2 w-5/12 md:block hidden" alt="">
      <div class="text-center  lg:w-1/2 md:w-7/12 w-full md:px-10">
        <p class="cinzel lg:text-5xl md:text-3xl text-xl mt-10 " style="font-weight: bold;">OPTIMIZE YOUR FACILITIES, ENHANCE YOUR BUSINESS</p>
        <p class="lg:my-10">At Teren FM we let you focus on your productivty and maximizing your profits as we easily
          manage your facilities</p>
        <div class="flex my-5 md:block hidden">
          <Button severity="info" @click="router.push('/about')" class="mx-auto w-3/4">Learn More</Button>
        </div>
      </div>
      <img src="/images/hero.png" class="lg:w-1/2 md:w-5/12 md:hidden block" alt="">
      <div class="flex my-5 md:hidden block">
          <Button severity="info" @click="router.push('/about')" class="mx-auto w-3/4">Learn More</Button>
        </div>
    </div>

    <!-- WHY CHOOSE US -->
    <div class="mt-10">
      <p class="text-center text-3xl font-bold md:block hidden">Why Teren</p>
      <heading title="Why Teren" class="md:hidden block"></heading>
      <div class="flex flex-wrap justify-around p-10">
        <div v-for="{ label, desc } in whyData" class="rounded bg-slate-200 lg:shadow-xl shadow shadow-slate-400 lg:w-3/12 md:w-5/12 lg:px-5 px-2 m-3">
          <div class="lg:w-3/4 w-10/12 mx-auto text-center">
            <p class="text-center   font-bold text-xl my-3">{{ label }}</p>
            <p class="my-5">{{ desc }}</p>
          </div>
        </div>
      </div>
      
    </div>

    <!-- SERVICES -->
    <services/>

    <!-- VALUES -->
     <value/>

     <!-- CTA -->
      <c-t-a></c-t-a>

  </main>
</template>
<style>
.cinzel {
  font-family: "Cinzel", serif;
  font-optical-sizing: auto;
  font-weight: 700;
  font-style: normal;
}
</style>
