<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container mx-auto p-4 flex justify-between">
                <nuxt-link class="font-bold" to="/">Nuxt Todo</nuxt-link>
            <!-- No Call to server to fetch pages -->
            <ul class="flex gap-4">
                <li><NuxtLink to="/">Home</NuxtLink></li>
                <li><NuxtLink to="/about">About</NuxtLink></li>
                <li><NuxtLink to="/products">Products</NuxtLink></li>
                <!-- here btn class is defined using tailwind -->
                <a href="/about" class="btn">About (ServerSide)</a>
            </ul>
            <!-- normal page serverside rendering.Can check in Network tab -->
        </nav>
        </header>

        <!-- output pages with this default layout and nuxt will automaticaly wrap pages with dafualt Layout -->

        <div class="container mx-auto p-4">
            <slot />
        </div>
    </div>
</template>

<style >

.router-link-exact-active{
    color: lightgreen;
}
</style>