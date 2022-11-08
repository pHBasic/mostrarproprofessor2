<template>
	<div class="container">
		<div class="container-about">
			<div class="wrapper-about">
				<h1 class="title">Professor de Física, Matemática e Química, Aulas Particulares e Reforço Escolar, Licenciado em Física UFS</h1>
				<div class="subtitle">Sergipe. Na casa dele. Em minha casa webcam.</div>
			</div>
			<div>
				<h2 class="title">Sobre a aula</h2>
				<p>
					Lucas ipsum dolor sit amet jinn palpatine c-3po fisto obi-wan windu darth hutt moff palpatine. Yavin lando baba kessel darth. Kamino antilles anakin ben fett. Skywalker coruscant hutt padmé darth luke mandalore jar. Yavin palpatine wampa solo maul luuke ahsoka obi-wan moff. Moff hutt lars fett wicket hutt. Mace obi-wan kenobi sidious skywalker luke. Wedge kashyyyk darth windu solo tatooine moff owen. Windu solo kenobi coruscant palpatine. Organa cade secura wookiee dooku wedge organa windu chewbacca.
					Skywalker windu boba amidala darth hutt kessel chewbacca. Biggs sidious antilles mara dantooine mon kenobi hutt. Skywalker calamari wampa solo ewok bothan darth ventress mothma. Utapau watto sidious obi-wan. Mothma jinn boba jinn biggs ahsoka skywalker dagobah lando. Darth mace yoda boba dooku cade. Solo gamorrean solo vader darth. Han jinn solo skywalker hutt han moff. C-3po lando utapau mon. Skywalker jade darth leia. Moff grievous dantooine mon ponda mon jinn leia. Mothma palpatine lando binks gamorrean.
					Dantooine jango yoda darth. Skywalker k-3po coruscant tatooine owen maul gonk. Owen maul binks antilles mara darth darth. Ventress darth lars anakin yavin mara. Alderaan solo antilles moff gonk kashyyyk moff jango jabba. Sebulba jabba darth solo hutt mustafar lobot. Dagobah sidious skywalker jabba windu. Ventress biggs jabba tatooine. Padmé jango c-3po dantooine dagobah. Moff ponda kenobi calrissian qui-gonn anakin jango padmé biggs. Jinn tatooine organa wedge kessel mon obi-wan calamari wookiee.
				</p>
			</div>
			<div>
			
			</div>
			<div>
				<h2 class="title">Mais sobre Palpatine</h2>
				<p>
					Lucas ipsum dolor sit amet jinn palpatine c-3po fisto obi-wan windu darth hutt moff palpatine. Yavin lando baba kessel darth. Kamino antilles anakin ben fett. Skywalker coruscant hutt padmé darth luke mandalore jar. Yavin palpatine wampa solo maul luuke ahsoka obi-wan moff. Moff hutt lars fett wicket hutt. Mace obi-wan kenobi sidious skywalker luke. Wedge kashyyyk darth windu solo tatooine moff owen. Windu solo kenobi coruscant palpatine. Organa cade secura wookiee dooku wedge organa windu chewbacca.
					Skywalker windu boba amidala darth hutt kessel chewbacca. Biggs sidious antilles mara dantooine mon kenobi hutt. Skywalker calamari wampa solo ewok bothan darth ventress mothma. Utapau watto sidious obi-wan. Mothma jinn boba jinn biggs ahsoka skywalker dagobah lando. Darth mace yoda boba dooku cade. Solo gamorrean solo vader darth. Han jinn solo skywalker hutt han moff. C-3po lando utapau mon. Skywalker jade darth leia. Moff grievous dantooine mon ponda mon jinn leia. Mothma palpatine lando binks gamorrean.
					Dantooine jango yoda darth. Skywalker k-3po coruscant tatooine owen maul gonk. Owen maul binks antilles mara darth darth. Ventress darth lars anakin yavin mara. Alderaan solo antilles moff gonk kashyyyk moff jango jabba. Sebulba jabba darth solo hutt mustafar lobot. Dagobah sidious skywalker jabba windu. Ventress biggs jabba tatooine. Padmé jango c-3po dantooine dagobah. Moff ponda kenobi calrissian qui-gonn anakin jango padmé biggs. Jinn tatooine organa wedge kessel mon obi-wan calamari wookiee.
				</p>
			</div>
		</div>
		<div class="container-request">
			<div class="card">
				<div class="perfil-wrapper">
					<div class="img"></div>
					<p class="name">Palpatine Skywalker</p>
				</div>
				<ul>
					<li>
						<span>Preço hora/aula</span>
						<span class="value">R$120</span>
					</li>
					<li>
						<span>Tempo de resposta</span>
						<span class="value">1h</span>
					</li>
					<li>
						<span>Número de alunos</span>
						<span class="value">34</span>
					</li>
				</ul>
			</div>
			<div class="wrapper-request">
				<h1 class="title">Solicite sua aula</h1>
				<h3>Informe o que deseja aprender com Palpatine</h3>
				<select>
					<option value="0">Escolha a materia:</option>
					<option value="1">Biologia</option>
					<option value="2">Química</option>
					<option value="3">Física</option>
					<option value="4">Inglês</option>
					<option value="5">Português</option>
				</select>
				<select>
					<option value="0">Escolha o assunto:</option>
					<option value="1">x</option>
					<option value="2">y</option>
					<option value="3">z</option>
					<option value="4">w</option>
					<option value="5">ç</option>
				</select>
				<form action="">
					<h3>Data da aula</h3>
					<div class="switch-field">
						<input type="radio" id="radio-one" name="switch-one" value="yes" checked/>
						<label for="radio-one">Com urgência</label>
						<input type="radio" id="radio-two" name="switch-one" value="no" />
						<label for="radio-two">Propor data</label>
					</div>
				</form>
				<DatePicker v-model="date" mode="dateTime" columns="1" :first-day-of-week="1" is24hr :minute-increment="60"/>
			</div>
		</div>
	</div>
</template>

<script>
  import { DatePicker } from 'v-calendar';
  import 'v-calendar/dist/style.css'
  
  export default {
	  components: {
		  DatePicker,
	  },
	}
</script>

<style scoped>
	.container {
		display: flex;
		flex-direction: row;
		padding: 15px;
	}
	.container-about {
		width: 60%;
		display: flex;
		flex-direction: column;
		justify-content: space-between;
		padding: 0 10px 0 10px;
	}
	.wrapper-about {
		background-color: #1A2DF320;
		border-radius: 10px;
		margin: 0 10px 15px 0;
		padding: 10px;
		box-shadow: 0 0 20px #ccc;
	}
	.container-request {
		padding: 0 10px 0 10px;
		width: 40%;
	}
	.card {
		display: flex;
		justify-content: center;
		box-shadow: 0 0 20px #ccc;
		min-height: 300px;
		width: 100%;
		margin-bottom: 50px;
		border-radius: 10px;
		align-items: center;
	}
	.perfil-wrapper {
		padding: 10px;
	}
	.img {
		height: 150px;
		width: 150px;
		background-image: url('../components/img/professor.jpeg');
		background-repeat: no-repeat;
		background-size: cover;
		background-position: center;
		margin: 0 0 0 0;
		border-radius: 5px;
		box-shadow: 0.5rem 0.5rem #ec146420, -0.5rem -0.5rem #1A2DF320;
		margin: auto;
	}
	.name {
		font-size: 20px;
	}
	ul {
		margin:  0 0 60px 10px;
		padding: 0;
	}
	li {
		list-style-type: none;
		padding-bottom: 10px;
	}
	.value {
		margin-left: 15px;
	}
	.wrapper-request {
		padding: 10px;
		background-color: #ec146420;
		border-radius: 10px;
		box-shadow: 0 0 20px #ccc;
	}
	.title {
		margin: 0;
		line-height: normal;	
		margin: 10px 0;
	}

	.switch-field {
		display: flex;
		margin-bottom: 36px;
		overflow: hidden;
	}

	.switch-field input {
		position: absolute !important;
		clip: rect(0, 0, 0, 0);
		height: 1px;
		width: 1px;
		border: 0;
		overflow: hidden;
	}

	.switch-field label {
		background-color: #e4e4e4;
		color: rgba(0, 0, 0, 0.6);
		font-size: 14px;
		line-height: 1;
		text-align: center;
		padding: 8px 16px;
		margin-right: -1px;
		border: 1px solid rgba(0, 0, 0, 0.2);
		box-shadow: inset 0 1px 3px rgba(0, 0, 0, 0.3), 0 1px rgba(255, 255, 255, 0.1);
		transition: all 0.1s ease-in-out;
	}

	.switch-field label:hover {
		cursor: pointer;
	}

	.switch-field input:checked + label {
		background-color: #1A2DF335;
		box-shadow: none;
	}

	.switch-field label:first-of-type {
		border-radius: 4px 0 0 4px;
	}

	.switch-field label:last-of-type {
		border-radius: 0 4px 4px 0;
	}


</style>
