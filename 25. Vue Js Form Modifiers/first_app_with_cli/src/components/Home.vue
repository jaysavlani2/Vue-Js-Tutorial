<template>
<h1>Form Modifiers</h1>
<input type="number" v-model.trim.lazy="data"/>
<h2>Data: {{ typeof(data) }}</h2>
<h2>Data: {{ data }}</h2>
</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
            data: ''
        }
    },
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
