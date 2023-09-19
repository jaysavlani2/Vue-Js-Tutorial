<template>
<h1>Slots</h1>
<Child></Child>
<Child>
    <h1>Code Step by step</h1>
</Child>
<Child>
    <a href="#">Code step by step</a>
</Child>
<Child>
    <img src="https://images.unsplash.com/photo-1575936123452-b67c3203c357?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80" alt="" />
</Child>
</template>

<script>
import Child from './Child.vue';
export default {
    name: 'Home',
    components: {
        Child
    },
    data() {
        return {
            count: 0
        }
    },
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
