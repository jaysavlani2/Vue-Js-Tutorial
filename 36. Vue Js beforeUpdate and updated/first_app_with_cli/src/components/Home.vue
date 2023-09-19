<template>
<h1>beforeUpdate and updated life cycle method</h1>
<h2 ref="count">Counter:{{ counter }}</h2>
<button v-on:click="update">Update Count</button>
</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
            counter: 0
        }
    },
    methods: {
        update() {
            this.counter +=1
        }
    },
    beforeUpdate() {
        console.log('Before Update', this.$refs['count'].textContent)
    },
    updated() {
        console.log('Updated', this.$refs['count'].textContent)
    }

}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
