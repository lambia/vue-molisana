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
	}
}
</script>

<template>
	<AppHeader />
	<main>
		<AppJumbo />
		<AppProdotti />
	</main>
	<AppFooter />
</template>

<style scoped></style>