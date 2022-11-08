<template>
  <div class="databloco">
  	<DatePicker v-model="date" mode="dateTime" columns="1" :first-day-of-week="1" is24hr />
		<div class="data">
			<h1>Data escolhida:</h1>
			 <p>{{ date.toLocaleString() }}</p>
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
	data() {
		return {
			date: new Date(),
		}
	}
}
</script>


<style scoped>

	.databloco{
		display: flex;
		flex-direction: column;
		align-items: center;

	}
	.data {
		display: flex;
		justify-content: space-between;
		align-items: center;
		border: solid #2196F3;
		color: #2196F3;
		padding: 5px;
		border-radius: 10px;
		width: fit-content;
		margin-top: 10px
	}

	.data h1 {
		font-size: medium;
	}
	
	.data p {
		margin-left: 3px;
	}
</style>