<template>
<h1>Watchers</h1>
<h2>Count: {{ count }}</h2>
<button v-on:click="count+=1">Plus</button>
<button v-on:click="count-=1">Minus</button>
</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
            count: 0
        }
    },
    watch: {
        count(val,prev) {
            if (val > 5 && val>prev) {
                alert('Stop Counting');
                this.count = 0
            }
            // alert('Value changed')
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
