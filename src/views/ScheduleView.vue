<template>
    <div class="wrapper-button">
        <!-- <ButtonComponent :pathRoute="route" :pathName="name" /> -->
        <!-- <ButtonComponent pathRoute="/agendar/student" pathName="Estudante" /> -->
        <RouterLink class="button" to="/agendar/professor">Professor</RouterLink>
    </div>

</template>

<script>
// import ButtonComponent from '../components/PathButtonComponent.vue'

// export default {
//     data: () => ({
//         route: '/agendar/professor',
//         name: 'Professor'
//     }),

//     components: {
//         ButtonComponent,
//     }
// }
</script>

<style scoped>
    .wrapper-button{
        display: flex;
		justify-content: center;
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
		margin: 100px 20px;
    }

    @media (hover:hover) {
        .button:hover {
            border-radius: 5px;
        }
    }
</style>