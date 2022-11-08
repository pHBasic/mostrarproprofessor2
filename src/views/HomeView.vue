<template>
    <div class="home">
        <Welcome />
        <RouterLink class="button" to="/agendar/listagem-professor">Encontre seu professor</RouterLink>
    </div>
</template>

<script>
import Welcome from '../components/WelcomeComponent.vue'

export default {
    components: {
        Welcome,
    }
}
</script>

<style scoped>
  .home{
    min-height: 100%;
		display: flex;
		flex-direction: column;
  }

	.button{
		background-color: #1A2DF3;
		color: white;
		border-radius: 10px;
		padding: 5px;
		width: 230px;
		font-size: 15pt;
		text-align: center;
		transition: 0.3s;
		margin: 25px 0;
		align-self: center;
	}

	@media (hover:hover) {
	.button:hover {
			border-radius: 5px;
	}
    }
</style>