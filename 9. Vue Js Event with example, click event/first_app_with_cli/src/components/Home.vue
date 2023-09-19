<template>
    <h1 v-on:mouseover="getConsole()">Home Component</h1>
    <button v-on:click="getData()">Click me</button>
    <button v-on:dblclick="getData('Button Double clicked')">Click me</button>
    <h2>{{ count }}</h2>
</template>

<script>
export default {
    name:'Home',
    data(){
        return {
            count: 0
        }
    },
    methods: {
        getData(){
            this.count = this.count+1
        },
        getConsole(){
            console.log('Mouse Over')
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>