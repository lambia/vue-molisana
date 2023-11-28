<script>
export default {
    name: "AppHeader",
    data() {
        return {
            menuLinks: [
                {
                    text: "Home",
                    url: "#home",
                },
                {
                    text: "Prodotti",
                    url: "#prodotti",
                },
                {
                    text: "Chi Siamo",
                    url: "#chisiamo",
                },
                {
                    text: "Contatti",
                    url: "#contatti",
                },
            ]
        }
    },
    mounted() {
        console.log("Componente AppHeader caricato");
    }
}
</script>

<template>
    <header>
        <nav>
            <a v-for="link in menuLinks" :href="link.url">{{ link.text }}</a>
        </nav>
    </header>
</template>

<style>
nav a {
    margin: 0 1rem;
}
</style>