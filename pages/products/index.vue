<template>
    <div>
        <h2>This is Product Page!!! and it using <span class="font-bold"> product layout</span></h2>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Pariatur sint dolorum doloribus voluptatem
            veritatis commodi modi vel molestias iste! Placeat mollitia reiciendis consequuntur fuga voluptas ex porro
            tempora, perferendis laboriosam?</p>
        <br>
        <!-- <h2>This route Path is : /product/{{ id }}</h2> -->
        <div class="grid grid-cols-4 gap-5">
            <div v-for="p in products">
                <ProductCard :product="p" />
            </div>
        </div>
    </div>
</template>

<script setup>
definePageMeta({
    layout: "products"
})
const { data: products } = await useFetch("https://fakestoreapi.com/products")
</script>

<style lang="scss" scoped></style>