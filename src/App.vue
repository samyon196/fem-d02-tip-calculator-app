<script setup>
import LightDarkToggle from './components/LightDarkToggle.vue'
</script>

<template>
    <LightDarkToggle />
    <div class="_main flex flex-col items-center">
        <img src="logo.svg" class="w-32" />
        <div class="_calcContainer bg-white dark:bg-gray-600 shadow rounded-3xl mx-auto my-60 p-8">Bill zzzz</div>
    </div>
</template>

<style>
body {
    @apply transition-colors bg-cyan-100 dark:bg-cyan-800;
}
</style>
