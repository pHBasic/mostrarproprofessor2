<template>
   <nav class="nav">
    <div class="wrapper-routes">
      <RouterLink class="routes" to="/">Início</RouterLink>
      <RouterLink class="routes" to="/about">Sobre</RouterLink>
      <RouterLink class="routes" to="/agendar">Agendar</RouterLink>
    </div>
      <RouterLink to="/" tag="div">
      <img src="../assets/education.svg" class="logo" width="100">
    </RouterLink>
    <div class="perfil-wrapper">
      <RouterLink class="user" to="/perfil">Pedro</RouterLink>
    </div>
   </nav>
</template>

<script>
export default {

}
</script>

<style scoped>
    .nav {
        display: flex;
        justify-content: space-between;
        align-items: center;
				padding: 10px 10px 0;
				height: 60px;
        /* background-color: #1A2DF3; */
    }
	.wrapper-routes {
    display: flex;
		justify-content: flex-start;
		margin-left: 10px;
		width: 25%;
	}
	.routes {
		margin-right: 10px;
		padding: 0 5px;
		font-size: 20px;
		font-weight: 500;
	}

    .perfil-wrapper {
      display: flex;
		  align-items: center;
		  justify-content: flex-end;
		  width: 25%;
		  margin-right: 20px;
    }
    .user {
		  font-size: 20px;
		  font-weight: 500;
		  padding: 0 5px;
    }
</style>