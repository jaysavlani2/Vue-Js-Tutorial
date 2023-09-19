<template>
<h1>beforeCreate and Created life cycle method {{ name }}</h1>
</template>

<script>
export default {
    name: 'Home',
    data() {
        console.log('created')
        return {
            name: 'Jay'
        }
    },
    beforeCreate() {
        // will not change name property
        this.name = 'Sam'
        alert('Before Create')
    },
    created() {
        // will change name property
        this.name = 'Mark'
        alert('Created')
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
