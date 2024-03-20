<template>
    <div>
        <h2>This is dynamic route</h2>
        <h2>This route Path is : /product/{{ id }}</h2>
    </div>
</template>

<script setup>
definePageMeta({
    layout: "products"
})

const { id } = useRoute().params

const url = "https://fakestoreapi.com/products" + id
const { data: product } = await useFetch(url, { key: id })

// below is for sending our product route to error.vue and funny thing is that its causing an issue and i mnot in mood of fixing it
// if (!product.value) {
//     throw createError({ message: "Product Not found", statusCode: 404 })
// }
</script>

<style lang="scss" scoped></style>