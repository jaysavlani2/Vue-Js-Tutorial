<template>
<h1>{{ item.email }} {{ item.name }}</h1>
<button v-on:click="getData(item)">Click Me</button>
</template>

<script>
export default {
    name: 'User',
    props: {
        item: {
            name: String,
            email: String
        },
        getData: Function
    }
}
</script>
