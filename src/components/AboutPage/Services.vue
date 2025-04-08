<script setup>
import Heading2 from '../Heading2.vue';
import { Accordion, AccordionPanel, AccordionHeader, AccordionContent } from 'primevue';
import IconPoint from '../icons/IconPoint.vue';

const services = [
    {
        value:0,
        label: "Hard Facilities Management Services",
        services: [
            "Planned Preventive & Reactive Maintenance",
            "HVAC (Heating, Ventilation & Air Conditioning) Management",
            "Electrical & Lighting Systems Maintenance",
            "Plumbing, Water, and Drainage Systems",
            "Fire Safety & Suppression Systems",
            "Building Fabric & Structural Maintenance",
            "Energy Management & Efficiency Solutions",
            "Generator & UPS Maintenance",
            "Elevator & Escalator Maintenance",
            "Health & Safety Compliance Inspections"
        ]
    },
    {
        value:1,
        label: "Soft Facilities Management Services",
        services: [
            "Cleaning & Janitorial Services",
            "Security & Access Control Management",
            "Waste Management & Recycling Solutions",
            "Landscaping & Grounds Maintenance",
            "Pest Control & Fumigation",
            "Front Desk & Reception Services",
            "Catering & Hospitality Services",
            "Office Support & Mailroom Services"
        ]
    },
    {
        value:2,
        label: "Workplace & Support Services",
        services: [
            "Helpdesk & Call Center Support",
            "Concierge & Visitor Management Services",
            "Meeting & Conference Room Management",
            "Space Planning & Office Moves",
            "Business Continuity & Emergency Planning",
            "Fleet & Transport Management"
        ]
    },
    {
        value:3,
        label: "Environmental & Sustainability Services",
        services: [
            "Waste Management & Recycling Programs",
            "Water Conservation & Treatment Solutions",
            "Carbon Footprint Reduction Strategies",
            "Green Building Maintenance & LEED Compliance",
            "Sustainable Procurement Solutions"
        ]
    },
    {
        value:4,
        label: "Technology & Smart FM Solutions",
        services: [
            "Building Management Systems (BMS)",
            "IoT-Based Predictive Maintenance",
            "CAFM (Computer-Aided Facility Management) Software",
            "AI-Driven Asset Optimization",
            "Smart Energy Monitoring & Automation"
        ]
    }
];
</script>
<template>
    <div class="mt-10">
        <heading2 title="Our Services" mini_title="Services"></heading2>
        <p class="text-center">Explore our diverse range of facilities management expertise.</p>
    </div>
    <div class="sm:w-3/4 mx-auto">
        <Accordion value="0">
            <AccordionPanel v-for="tab in services" :key="tab.title" :value="tab.value">
                <AccordionHeader><span class="text-xl">{{ tab.label }}</span></AccordionHeader>
                <AccordionContent>
                    <div class="grid md:grid-cols-2  gap-5">
                        <div class="flex items-center" v-for="service in tab.services">
                            <component :is="IconPoint"></component>
                            <p class="m-0" >{{ service }}</p>
                        </div>
                    </div>
                    
                </AccordionContent>
            </AccordionPanel>
        </Accordion>
    </div>
</template>