<template>
<h1>Send child to parent data component</h1>
<h1>User Name: {{ childUser }}</h1>
<User :getUserName="getUserName"/>
</template>

<script>
import User from './User.vue';
export default {
    name: 'Home',
    components: {
        User
    },
    data() {
        return {
            childUser: ''
        }
    },
    methods: {
        getUserName(name) {
            this.childUser = name
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
