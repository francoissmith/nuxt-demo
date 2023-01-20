<template>
    <div>
        <header class="shaddow-sm bg-white">
            <nav class="container mx-auto p-4 flex justify-between">
                <NuxtLink to="/" class="font-bold">Demo Nuxt</NuxtLink>
                <ul class="flex gap-4">
                    <li><NuxtLink to="/">Home</NuxtLink></li>
                    <li><NuxtLink to="/about">About</NuxtLink></li>
                    <li><NuxtLink to="/products" class="btn">Products</NuxtLink></li>
                </ul>
            </nav>
        </header>

        <!-- output content -->
        <div class="container mx-auto p-4">
            <slot/>
        </div>
    </div>
</template>

<style scoped>
.router-link-exact-active {
    color: darkcyan;
}
</style>