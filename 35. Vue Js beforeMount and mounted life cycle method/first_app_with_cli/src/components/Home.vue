<template>
<h1>beforeMount and mounted life cycle method</h1>
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
    },
    beforeMount() {
        // Element will be null as it is not yet mounted
        console.log('beforeMount', this.$el);
    },
    mounted() {
         // Element will not be null as it is already mounted
         console.log('mounted', this.$el);
    }

}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
