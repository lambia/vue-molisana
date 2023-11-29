<script>
import AppCard from './AppCard.vue'

export default {
    name: "AppProdotti",
    props: ["products", "titolo"],
    components: {
        AppCard
    }
}
</script>

<template>
    <section>
        <h2>{{ titolo }}</h2>
        <div id="cardsWrapper">
            <AppCard v-for="prodotto in products" :product="prodotto" />
        </div>
    </section>
</template>

<style scoped>
section {
    background: #DDD;
}

#cardsWrapper {
    display: flex;
    flex-wrap: wrap;
}
</style>