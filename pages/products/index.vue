<template>
    <div>
        <div class="grid grid-cols-4 gap-5">
            <div v-for="p in products">
                <ProductCard :product="p"/>
            </div>
        </div>
    </div>
</template>

<script setup>
    definePageMeta({
        layout: 'products'
    });

    // fetch products
    const { data: products } = await useFetch('https://fakestoreapi.com/products');

    useHead({
        title: 'Nuxt Demo | Shop',
        meta: [
            { name: 'description', content: 'Nuxt 3 Shop'}
        ]
    })
</script>

<style scoped>

</style>