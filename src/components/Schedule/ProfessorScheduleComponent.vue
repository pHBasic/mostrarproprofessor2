<template>
	<div class="databloco">
		<DatePicker v-model="date" mode="dateTime" columns="1" :first-day-of-week="1" is24hr :minute-increment="60"/>
		  <div class="data">
				<h1>Informações da Aula</h1>
			   <p><strong>Data:</strong> {{ date.toLocaleString() }}</p>
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
		let date = new Date();
		date.setMinutes(0, 0, 0);
		  return {
			  date,
		  }
	  }
  }
  </script>
  
  
  <style scoped>
	  .databloco{
		  display: flex;
		  align-items: flex-start;
		  border: solid #545454;
		  padding: 5px;
  
	  }
	  .data {
		  display: flex;
		  justify-content: space-between;
		  align-items: center;
		  /* border: solid #2196F3; */
		  color:var(--gray-900);
		  padding: 5px;
		  border-radius: 10px;
		  width: fit-content;
		  margin-top: 10px
	  }
  
	  .data h2 {
		  font-size: medium;
	  }
	  
	  .data p {
		  margin-left: 3px;
	  }
  </style>