<template>
    <Head>
        <Title>About Page</Title>
        <Meta name="description" content="About Page Description"></Meta>
        <!-- <Meta name="description" :content={{ some dynamic value }}></Meta> -->
    </Head>
    <div>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti earum minima ut exercitationem veniam!
            Doloribus tenetur aspernatur, vero, nesciunt saepe odio sed magni accusantium accusamus sit impedit
            repudiandae minus illo.</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti earum minima ut exercitationem veniam!
            Doloribus tenetur aspernatur, vero, nesciunt saepe odio sed magni accusantium accusamus sit impedit
            repudiandae minus illo.</p>
    </div>
</template>

<script setup>
useHead({
    title: "Nuxt Dojo | About",
    meta: [
        { name: "About Description", content: "Eveything is Description" }
    ]
})
</script>

<style scoped></style>