<template>
	<header>
		<Navbar/>
	</header>
	<div class="body">
		<RouterView />
	</div>
	<footer class="rodape">
		<FooterComponent />
	</footer>
</template>

<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Navbar from './components/NavbarComponent.vue';
import FooterComponent from './components/FooterComponent.vue';
</script>

<style scoped>
	.body {
	}
	.rodape {
		display: block;
	}

</style>
