<template>
    <h1>Child Component</h1>
    <h1>{{ name }}</h1>
    <h2>{{ user.name }}</h2>
    <h2>{{ user.email }}</h2>
    <button v-on:click="getData()">Call Function</button>
</template>

<script>
export default  {
    name:'Child',
    props:{
        name: String,
        user: {
            name: String,
            email: String
        },
        getData: Function
    }
}
</script>