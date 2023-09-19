<template>
<h1>beforeUnmount and unmounted life cycle method</h1>
<User v-if="show"/>
<button v-on:click="show=!show">Hide</button>
</template>

<script>
import User from './User.vue';
export default {
    name: 'Home',
    components: {
        User,
    },
    data() {
        return {
            show: true
        }
    },
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
