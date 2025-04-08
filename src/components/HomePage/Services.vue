<script setup>
import Heading from '../Heading.vue';
const services = [
    {
        label:'HARD FACILITIES MANAGEMENT',
        description:"We ensure your building's infrastructure operates at peak performance. Our hard FM services cover everything from essential maintenance to complex systems management, ensuring safety, compliance, and efficiency",
        image:'/images/services/hardfm.png'
    },
    {
        label:'SOFT FACILITIES MANAGEMENT',
        description:"Our  services focus on creating a comfortable, safe, and productive environment for your occupants. We handle everything from cleaning and security to catering and office support, enhancing workplace experience.",
        image:'/images/services/softfm.png'
    },
    {
        label:'Workplace & Support Services',
        description:"We provide essential support services to optimize your workplace operations. From helpdesk support and visitor management to space planning and emergency preparedness, we ensure a smooth and efficient workflow.",
        image:'/images/services/workplacefm.png'
    },
    {
        label:'Environmental & Sustainability Services',
        description:"We are committed to sustainable practices that minimize environmental impact and promote resource efficiency. Our services include waste reduction, energy conservation, and green building maintenance, helping you achieve your sustainability goals",
        image:'/images/services/environmentalfm.png'
    },
    {
        label:'Technology & Smart FM Solutions',
        description:"We leverage cutting-edge technology to optimize facility operations and enhance efficiency. Our smart FM solutions include building management systems, predictive maintenance, and AI-driven optimization for data-driven decision-making.",
        image:'/images/services/technologyfm.png'
    },
]
</script>

<template>
    <main>
            <heading  title="Our Services" mini_title="Services"></heading>
            <div  class="md:px-20 px-10 lg:my-4 my-10" v-for="({label,description,image},i) in services" :key="i">
                <div class="lg:flex" :class="i%2 != 0 ? 'flex-row-reverse' : ''">
                    <img :src="image" class="lg:w-1/2 w-5/12 float-right h-1/2 lg:block hidden" alt="">
                    <div class="text-center lg:w-1/2 w-full flex items-center">
                        <div>
                            <img :src="image" class="lg:w-1/2 w-5/12 md:block hidden lg:hidden  h-1/2" :class="i%2 != 0 ? 'float-right' : 'float-left'" alt="">
                            <p class="lora g:text-4xl text-2xl px-4 leading-10 lg:mb-10">{{ label }}</p>
                            <img :src="image" class="lg:w-1/2 md:w-5/12 md:hidden block  h-1/2"  alt="">
                            
                            <p class="md:px-10 lg:leading-10">{{ description }}</p>
                        </div>
                    </div>
                </div>
            </div>
        
    </main>
</template>

<style>
.lora {
  font-family: "Lora", serif;
  font-optical-sizing: auto;
  font-weight: 700;
  font-style: normal;
}

</style>