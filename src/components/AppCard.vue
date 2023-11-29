<script>
export default {
    // props: ["product"]
    props: {
        product: Object
    }
}
</script>

<template>
    <div class="card">
        <h3>{{ product.titolo }}</h3>
        <p>Pasta {{ product.tipo }}</p>
        <p>Tempo di cottura: {{ product.cottura }} minuti</p>
        <img :src="product.src" alt="">
    </div>
</template>

<style scoped>
.card {
    background: white;
    border: solid 1px #CCC;
    padding: 1rem;
    margin: 1rem;
    width: 30%;
}

img {
    width: 100%;
}
</style>