<template>
    <div>
        <h2>About</h2>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Molestias autem consequuntur reprehenderit
            consequatur beatae fuga sed doloribus quae pariatur quis, facilis facere, expedita, consectetur architecto.
            Id voluptates dicta illo eos!</p>

        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Molestias autem consequuntur reprehenderit
            consequatur beatae fuga sed doloribus quae pariatur quis, facilis facere, expedita, consectetur architecto.
            Id voluptates dicta illo eos!</p>

        <div>{{ data }}</div>
    </div>
</template>

<script setup>
const { data } = await useFetch('/api/currency/ZAR');
</script>

<style scoped>
h2 {
    margin-top: 20px;
    font-size: 36px;
}

p {
    margin: 20px 0;
}
</style>