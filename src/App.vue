<script>
import AppHeader from './components/AppHeader.vue'
import AppJumbo from './components/AppJumbo.vue'
import AppProdotti from './components/AppProdotti.vue'
import AppFooter from './components/AppFooter.vue'

export default {
	components: {
		AppHeader,
		AppJumbo,
		AppProdotti,
		AppFooter,
	},
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
			],
			pastaCorta: [
				{
					src: "https://www.lamolisana.it/wp-content/uploads/2021/05/38-mezze-maniche.jpg",
					titolo: "N.38 Mezze maniche",
					tipo: "corta",
					cottura: 12,
				},
				{
					src: "https://www.lamolisana.it/wp-content/uploads/2021/05/44-sedani.jpg",
					titolo: "N.44 Sedani",
					tipo: "corta",
					cottura: 8,
				},
				{
					src: "https://www.lamolisana.it/wp-content/uploads/2021/05/49-sedani.jpg",
					titolo: "N.49 Sedanini",
					tipo: "corta",
					cottura: 8,
				},
				{
					src: "https://www.lamolisana.it/wp-content/uploads/2021/05/53-lumachine.jpg",
					titolo: "N.53 Lumachine",
					tipo: "corta",
					cottura: 12,
				},
				{
					src: "https://www.lamolisana.it/wp-content/uploads/2021/05/55-chifferi-rigati.jpg",
					titolo: "N.55 Chifferi rigati",
					tipo: "corta",
					cottura: 12,
				},
				{
					src: "https://www.lamolisana.it/wp-content/uploads/2021/05/58-misto-corto.jpg",
					titolo: "N.58 Misto corto",
					tipo: "corta",
					cottura: 9,
				},
				{
					src: "https://www.lamolisana.it/wp-content/uploads/2021/06/84-ditale-quadrato.jpg",
					titolo: "N.84 Ditale Quadrato",
					tipo: "cortissima",
					cottura: 12,
				},
			],
			pastaLunga: [
				{
					src: "https://www.lamolisana.it/wp-content/uploads/2021/04/1-spaghetto-quadrato.jpg",
					titolo: "N.4 Spaghetto Quadrato Bucato",
					tipo: "lunga",
					cottura: 6,
				},
				{
					src: "https://www.lamolisana.it/wp-content/uploads/2021/04/5-fettuccine.jpg",
					titolo: "N.5 Fettuccine",
					tipo: "lunga",
					cottura: 13,
				},
				{
					src: "https://www.lamolisana.it/wp-content/uploads/2021/04/6-linguine.jpg",
					titolo: "N.6 Linguine",
					tipo: "lunga",
					cottura: 12,
				},
				{
					src: "https://www.lamolisana.it/wp-content/uploads/2021/04/7-mezze-linguine.jpg",
					titolo: "N.7 Mezze Linguine",
					tipo: "lunga",
					cottura: 11,
				},
				{
					src: "https://www.lamolisana.it/wp-content/uploads/2021/04/11-spaghettino-quadrato.jpg",
					titolo: "n.11 Spaghettino Quadrato",
					tipo: "lunga",
					cottura: 9,
				}
			]
		}
	}
}
</script>

<template>
	<AppHeader :links="menuLinks" />
	<main>
		<!-- Esempio di utilizzo font-awesome -->
		<!-- <font-awesome-icon icon="fa-solid fa-home" class="coloreRosso" /> -->
		<AppJumbo />
		<AppProdotti :products="pastaLunga" titolo="La nostra pasta lunga" />
		<AppProdotti :products="pastaCorta" titolo="La nostra pasta corta" />
	</main>
	<AppFooter />
</template>

<style scoped>
.coloreRosso {
	color: red;
}
</style>