<template>
    <h1>Get Input Field</h1>
    <input type="text" placeholder="Enter Email" v-model="email"/><br/><br/>
    <input type="password" placeholder="Enter Password" v-model="password"/><br/><br/>
    <button v-on:click="getData()" type="button">Get Values</button>
</template>

<script>
export default {
    name:'Home',
    data(){
        return {
            email: '',
            password: ''
        }
    },
    methods: {
        getData(){
            console.log('values:', this.email, this.password)
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>