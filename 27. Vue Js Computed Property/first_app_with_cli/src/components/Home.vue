<template>
<h1>Computed Property</h1>
<h2>{{getResult }}</h2>
<h2>{{getResult }}</h2>
<h2>{{getResultMethods() }}</h2>
</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
            dollars: 100,
            rupeeVal: 70,
            discount: 10
        }
    },
    methods: {
        getResultMethods() {
            return (this.dollars * this.rupeeVal) - this.discount
        }
    },
    computed: {
        getResult() {
            return (this.dollars * this.rupeeVal) - this.discount
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
