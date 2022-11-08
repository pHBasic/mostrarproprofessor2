<template>
    <a @click="fade()">{{ this.pathName }}</a>
</template>

<script>
import router from '../router';

export default {
    name: RouteButton,

    props: {
        pathRoute: String,
        pathName: String,
    },
    methods: {
        fade(){
            router.push(this.pathRoute);
        }
    }
}
</script>