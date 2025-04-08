<script setup>
const props = defineProps({title:String,mini_title:String})
</script>

<template>
    <main class="my-5">
        <p class=" px-5 lora-mini py-2 rounded-2xl w-fit mx-auto bg-blue-400">{{ mini_title }}</p>
        <h2 class="lora-title text-center text-5xl my-5">{{ title }}</h2>
    </main>
</template>

<style>
.lora-mini {
  font-family: "Lora", serif;
  font-optical-sizing: auto;
  font-weight: 500;
  font-style: normal;
}
.lora-title {
  font-family: "Lora", serif;
  font-optical-sizing: auto;
  font-weight: 500;
  font-style: normal;
}
</style>