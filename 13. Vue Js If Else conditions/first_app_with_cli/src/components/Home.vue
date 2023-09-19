<template>
<h1 v-if="show">If Condition</h1>
<h1 v-else>Else Condition</h1>
<button v-on:click="show=!show">Show</button>
</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
            show: true
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
