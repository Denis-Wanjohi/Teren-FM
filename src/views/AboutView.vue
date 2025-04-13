<script setup>
import Heading2 from '@/components/Heading2.vue';
import Services from '@/components/AboutPage/Services.vue';
import Serve from '@/components/AboutPage/Serve.vue';
import CTA from '@/components/CTA.vue';
import { onMounted } from 'vue';
onMounted(()=>{
  window.scrollTo(0, 0);
})
</script>
<template>
  <main>
    <!-- HERO -->
     <div class="text-center md:px-20 px-5">
      <p class="cinzel md:text-5xl text-2xl md:py-10 pt-10" style="font-weight:500;">Your Trusted Partner for Integrated Facilities Management </p>
      <p class="lora py-5" style="font-weight: 400;">Teren Facilities Management Limited is a trusted partner providing integrated facilities management (IFM) solutions . We deliver both hard and soft FM services to businesses, institutions, and property owners, ensuring efficient, safe, and sustainable operations.</p>
      <img src="/images/AboutPage/hero.png" alt="">
    </div>

    <!-- VISION AND MISSION -->
     <div class="md:flex px-5">
      <div class="lg:w-1/2 flex items-center">
        <div>
          <heading2 title="Our Vision" mini_title="Vision"></heading2>
        <img src="/images/AboutPage/vision.png" class="w-1/2 float-left md:hidden block" alt="">

        <p class="text-center lg:leading-10 lg:px-20 pl-5">To create a future where all facilities operate seamlessly and sustainably. We envision being the driving force behind optimized environments that enhance productivity, well-being, and environmental responsibility.        </p>
        </div>
      </div>
      <div class="lg:w-1/2 flex item-center md:block hidden">
        <img src="/images/AboutPage/vision.png" alt="">
      </div>
     </div>

     <div class="md:flex flex-row-reverse items-center px-5">
      <div class="lg:w-1/2 flex items-center">
        <div>
          <heading2 title="Our Mission" mini_title="Mission"></heading2>
          <img src="/images/AboutPage/mission.png" class="w-1/2 float-right md:hidden block" alt="">
        <p class="text-center lg:leading-10 lg:px-20 pr-5">To provide tailored facilities management services that meet the unique needs of each client, delivering value through cost optimization, innovative solutions, and a commitment to sustainability and compliance in all our operations. </p>
        </div>
      </div>
      <div class="lg:w-1/2 flex items-center pt-10 md:block hidden">
        <img src="/images/AboutPage/mission.png" class="" alt="">
      </div>
     </div>


     <!-- SERVICES -->
      <services class="mt-10"></services>

      <!-- SERVE -->
       <Serve></Serve>

       <!-- CTA -->
        <c-t-a></c-t-a>
  </main>
</template>

<style>

</style>
