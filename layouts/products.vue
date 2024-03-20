<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container mx-auto p-4 ">
                <nuxt-link class="font-bold" to="/">Nuxt Todo</nuxt-link>
            </nav>
        </header>
        
        <div class="container mx-auto p-4">
            <slot />
            <h1 class="font-bold">This Line is coming from layouts/product.vue </h1>
        </div>

        <footer class="container mx-auto p-4 flex justify-between border-t-2">
            <ul class="flex gap-4">
                <li>
                    <NuxtLink to="/">Home</NuxtLink>
                </li>
                <li>
                    <NuxtLink to="/about">About</NuxtLink>
                </li>
                <li>
                    <NuxtLink to="/products">Products</NuxtLink>
                </li>
            </ul>
        </footer>
    </div>
</template>
