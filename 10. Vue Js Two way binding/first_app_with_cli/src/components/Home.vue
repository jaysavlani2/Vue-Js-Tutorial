<template>
    <h1>Two way Binding</h1>
    <input type="text" v-model="count"/>
    <h2>{{ count }}</h2>
</template>

<script>
export default {
    name:'Home',
    data(){
        return {
            count: 10
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>