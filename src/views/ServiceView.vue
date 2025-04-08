<script setup>
import { Accordion, AccordionPanel, AccordionHeader, AccordionContent } from 'primevue';
import CTA from '@/components/CTA.vue';
const services = [
    {

        title: 'HARD FACILITIES MANAGEMENT',
        description: "Our hard facilities management ensures the reliable operation of your building's essential systems. We deliver expert maintenance, HVAC management, electrical systems, plumbing, and structural services, guaranteeing safety, compliance, and efficiency for uninterrupted operations",
        image: '/images/services/hardfm.png',
        services: [
            {
                value: 0,
                label: "Planned Preventive & Reactive Maintenance",
                description:
                    "Ensuring operational efficiency and minimizing downtime through proactive maintenance schedules and rapid response to breakdowns, preserving asset value and optimizing performance.",
            },
            {
                value: 1,
                label: "HVAC (Heating, Ventilation & Air Conditioning) Management",
                description:
                    "Maintaining optimal indoor environments for comfort, health, and productivity, while maximizing energy efficiency and minimizing operational costs through expert system management.",
            },
            {
                value: 2,
                label: "Electrical & Lighting Systems Maintenance",
                description:
                    "Ensuring safe, reliable, and energy-efficient electrical and lighting systems through regular inspections, maintenance, and upgrades, minimizing disruptions and enhancing workplace safety.",
            },
            {
                value: 3,
                label: "Energy Management & Efficiency Solutions",
                description:
                    "Optimizing energy consumption to reduce costs and environmental impact, implementing sustainable practices, and leveraging technology to enhance energy efficiency and minimize waste.",
            },
            {
                value: 4,
                label: "Plumbing, Water, and Drainage Systems",
                description:
                    "Maintaining efficient water distribution, waste removal, and drainage systems to prevent leaks, contamination, and structural damage, ensuring a healthy and hygienic environment.",
            },
            {
                value: 5,
                label: " Fire Safety & Suppression Systems",
                description:
                    "Protecting lives and property through comprehensive fire safety solutions, including prevention, detection, suppression, and compliance with all safety regulations and standards.",
            },
            {
                value: 6,
                label: "Building Fabric & Structural Maintenance",
                description:
                    "Preserving the integrity, safety, and aesthetic appeal of buildings through expert maintenance of structural elements, exteriors, and interiors, ensuring longevity and minimizing repair costs.",
            },
            {
                value: 7,
                label: "Generator & UPS Maintenance",
                description:
                    "Ensuring uninterrupted power supply during outages through reliable maintenance of backup generators and UPS systems, guaranteeing business continuity and minimizing downtime.",
            },
            {
                value: 8,
                label: "Health & Safety Compliance Inspections",
                description:
                    "Ensuring facilities meet all health and safety regulations, minimizing risks, preventing accidents, and creating a safe and compliant environment for all occupants",
            },
            {
                value: 9,
                label: "Elevator & Escalator Maintenance",
                description:
                    "Maintaining the safe and efficient operation of vertical transportation systems through regular inspections, repairs, and modernization, ensuring accessibility and a positive user experience.",
            },
        ]
    },
    {
        title: "SOFT FACILITIES MANAGEMENT",
        description: "Our soft FM services focus on creating a comfortable, safe, and productive environment for your occupants. We handle cleaning, security, waste management, landscaping, and office support, enhancing workplace experience and well-being.",
        image: '/images/services/softfm.png',
        services: [
            {
                value: 0,
                label: "Cleaning & Janitorial Services",
                description:
                    "Maintaining clean, healthy, and welcoming environments through comprehensive cleaning solutions, enhancing hygiene, promoting well-being, and creating a positive impression.",
            },
            {
                value: 1,
                label: "Security & Access Control Management",
                description:
                    "Protecting people, assets, and information through robust security measures, including access control, surveillance, and trained personnel, ensuring a safe and secure environment.",
            },
            {
                value: 2,
                label: "Waste Management & Recycling Solutions",
                description:
                    "Implementing sustainable waste management practices, minimizing environmental impact, promoting recycling, and ensuring responsible disposal in compliance with regulations.",
            },
            {
                value: 3,
                label: "Landscaping & Grounds Maintenance",
                description:
                    "Enhancing the aesthetic appeal and functionality of outdoor spaces through professional landscaping, groundskeeping, and maintenance, creating attractive and welcoming environments.",
            },
            {
                value: 4,
                label: "Pest Control & Fumigation",
                description:
                    "Protecting facilities from pests and infestations through effective prevention and elimination strategies, ensuring a healthy and hygienic environment for occupants and operations.",
            },
            {
                value: 5,
                label: "Front Desk & Reception Services",
                description:
                    "Providing professional and welcoming front desk services, managing visitors, handling inquiries, and ensuring efficient communication and a positive first impression for guests and clients.",
            },
            {
                value: 6,
                label: "Catering & Hospitality Services",
                description:
                    "Offering customized catering and hospitality solutions to enhance workplace experiences, providing quality food services, event support, and creating a welcoming and productive environment.",
            },
            {
                value: 7,
                label: "Office Support & Mailroom Services",
                description:
                    "Providing essential office support services, including mail handling, document management, and administrative assistance, streamlining operations and improving workplace efficiency.",
            },
        ],
    },
    {

        title: "Workplace and Support Services",
        description: "We provide essential support services to optimize your workplace operations. From helpdesk support and visitor management to space planning and emergency preparedness, we ensure a smooth and efficient workflow, enhancing productivity and collaboration.",
        image: '/images/services/workplacefm.png',
        services: [
            {
                value: 0,
                label: "Helpdesk & Call Center Support",
                description:
                    "Providing efficient and responsive support for facility-related requests, inquiries, and issues, ensuring prompt resolution and a positive user experience for all occupants.",
            },
            {
                value: 1,
                label: "Concierge & Visitor Management Services",
                description:
                    "Creating a welcoming and efficient experience for visitors through professional concierge services, managing access, providing information, and ensuring seamless visitor flow.",
            },
            {
                value: 2,
                label: "Meeting & Conference Room Management",
                description:
                    "Ensuring seamless management and operation of meeting and conference facilities, including scheduling, setup, technology support, and catering coordination for productive meetings.",
            },
            {
                value: 3,
                label: "Space Planning & Office Moves",
                description:
                    "Optimizing workspace utilization and managing efficient office relocations, ensuring minimal disruption, maximizing productivity, and creating functional and inspiring work environments.",
            },
            {
                value: 4,
                label: "Business Continuity & Emergency Planning",
                description:
                    "Developing and implementing comprehensive plans to ensure business resilience and minimize disruptions during emergencies, protecting people, assets, and operations through proactive preparedness.",
            },
            {
                value: 5,
                label: "Fleet & Transport Management",
                description:
                    "Managing company vehicles and transportation logistics efficiently, optimizing routes, ensuring vehicle maintenance, and providing reliable transportation solutions for staff and operations.",
            },
        ],
    },
    {

        title: "Environmental and Sustainability Services",
        description: "We are committed to sustainable practices that minimize environmental impact and promote resource efficiency. Our services include waste reduction, energy conservation, green building maintenance, and sustainable procurement, helping you achieve your sustainability goals.",
        image: '/images/services/environmentalfm.png',
        services: [
            {
                value: 0,
                label: "Waste Management & Recycling Programs",
                description:
                    "Implementing sustainable waste reduction and recycling initiatives, minimizing environmental impact, promoting responsible waste disposal, and achieving sustainability goals.",
            },
            {
                value: 1,
                label: "Water Conservation & Treatment Solutions",
                description:
                    "Reducing water consumption and ensuring water quality through efficient water management practices, implementing conservation strategies, and providing water treatment solutions.",
            },
            {
                value: 2,
                label: "Carbon Footprint Reduction Strategies",
                description:
                    "Implementing strategies to minimize an organization's environmental impact, reducing carbon emissions, promoting energy efficiency, and contributing to a sustainable future.",
            },
            {
                value: 3,
                label: "Green Building Maintenance & LEED Compliance",
                description:
                    "Maintaining green buildings to optimize performance, achieve LEED certification, and ensure sustainable operations through specialized maintenance practices and adherence to green building standards.",
            },
            {
                value: 4,
                label: "Sustainable Procurement Solutions",
                description:
                    "Integrating sustainable practices into procurement processes, selecting environmentally friendly products and suppliers, and promoting responsible sourcing to minimize environmental impact.",
            },
        ],
    },
    {

        title: "Technology and Smart FM Solutions",
        description: "We leverage cutting-edge technology to optimize facility operations and enhance efficiency. Our smart FM solutions include building management systems, predictive maintenance, CAFM software, and AI-driven optimization for data-driven decision-making and automation",
        image: '/images/services/technologyfm.png',
        services: [
            {
                value: 0,
                label: "Building Management Systems (BMS)",
                description:
                    "Utilizing technology to monitor and control building systems, optimizing performance, enhancing efficiency, and improving occupant comfort through centralized management and automation.",
            },
            {
                value: 1,
                label: "IoT-Based Predictive Maintenance",
                description:
                    "Leveraging IoT technology to anticipate maintenance needs, prevent equipment failures, minimize downtime, and optimize asset performance through proactive monitoring and data analysis.",
            },
            {
                value: 2,
                label: "CAFM (Computer-Aided Facility Management) Software",
                description:
                    "Using software to streamline facility management operations, improve efficiency, enhance communication, and optimize resource allocation through centralized data management and workflow automation.",
            },
            {
                value: 3,
                label: "AI-Driven Asset Optimization",
                description:
                    "Employing artificial intelligence to optimize asset performance, extend lifecycles, and reduce operational costs through data-driven insights, predictive analytics, and automated decision-making.",
            },
            {
                value: 4,
                label: "Smart Energy Monitoring & Automation",
                description:
                    "Implementing smart technologies to monitor and automate energy usage, maximizing energy efficiency, reducing consumption, and minimizing costs through intelligent c",
            },
        ],
    }
]
</script>

<template>
    <p class="lora md:text-6xl text-3xl text-center my-10" style="font-weight: 500;">OUR SERVICES</p>
    <main class="px-3">
        <div v-for="{ title, description, image, services } in services">
            <p class="cinzel text-center md:text-2xl text-xl my-5" style="font-weight: bold;">{{ title }}</p>
            <p class="text-center md:w-3/4 w-10/12 mx-auto">{{ description }}</p>
            <img :src="image" class="mx-auto md:w-[500px] w-10/12 my-5" alt="">
            <div class="sm:w-3/4  mx-auto">
                <Accordion value="0">
                    <AccordionPanel v-for="tab in services" :key="tab.title" :value="tab.value">
                        <AccordionHeader><span class="lg:text-2xl text-black">{{ tab.label }}</span></AccordionHeader>
                        <AccordionContent>
                            <p class="text-center"> {{ tab.description }}</p>
                        </AccordionContent>
                    </AccordionPanel>
                </Accordion>
            </div>
        </div>
    </main>
    <c-t-a></c-t-a>
</template>