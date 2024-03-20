<template>
    <div class="text-center">
        <h1 class="mt-7 text-7xl font-bold">{{ error.statusCode }}</h1>
        <p class="mt-7 text-6xl">Ooops</p>
        <h1 class="mt-7">{{ error.message }}</h1>
    </div>
</template>

<script setup>
defineProps(["error"])
</script>

<style scoped></style>