<script setup>
import IconCost from '../icons/IconCost.vue';
import IconSustainability from '../icons/IconSustainability.vue';
import IconInnovation from '../icons/IconInnovation.vue';
import IconCustomers from '../icons/IconCustomers.vue';
import Heading from '../Heading.vue';
const values = [
    {
        icon:IconCustomers,
        title:'Customer-centric services',
        description:'Tailored solutions that align with client needs.',
    },
    {
        icon:IconInnovation,
        title:'Innovation and technology',
        description:'Implementing smart FM solutions for efficiency.',
    },
    {
        icon:IconSustainability,
        title:'Sustainability and Compliance',
        description:'Adhering to industry standards and green practices.',
    },
    {
        icon:IconCost,
        title:'Cost Optimization',
        description:'Delivering value while reducing operational costs.',
    }
]
</script>

<template>
    <heading title="Our Values" mini_title="Values"></heading>
    <main class="grid md:grid-cols-2 ">
        <div v-for="{icon,title,description} in values" class="mx-auto border rounded-2xl md:p-10 p-5 m-5 w-3/4">
            <component :is="icon"></component>
            <h2 class="lora text-2xl">{{ title }}</h2>
            <p>{{ description }}</p>
        </div>
    </main>
</template>