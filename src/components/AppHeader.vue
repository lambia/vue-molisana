<script>
export default {
    name: "AppHeader",
    props: ["links"],
    mounted() {
        console.log("Componente AppHeader caricato");
    }
}
</script>

<template>
    <header>
        <nav>
            <a v-for="link in links" :href="link.url">{{ link.text }}</a>
        </nav>
    </header>
</template>

<style scoped>
nav a {
    margin: 0 1rem;
}
</style>