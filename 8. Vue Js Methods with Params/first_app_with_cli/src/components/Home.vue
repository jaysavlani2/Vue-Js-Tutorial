<template>
    <h1>Email: {{ email }}</h1>
    <h1>Name: {{ getName('Jay') }}</h1>
    <h1>All Data Email: {{ getData().email }} </h1>
    <h1>All Data Name: {{ getData().name }} </h1>
</template>

<script>
export default {
    name:'Home',
    data(){
        return {
            email: 'jaysavlani2@gmail.com',
        }
    },
    methods: {
        getName(name) {
            return name
        },
        getData() {
            return { 
                name: 'Jay',
                email: this.email,
            }
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>