<template>
<h1>Multiple slots with Slots Name</h1>
<Child>
    <template v-slot:header>
        <h1>Jay</h1>
    </template>
    <template v-slot:content>
        <p>A Vue Js Product</p>
    </template>
    <template v-slot:footer>
        <button>Click Me</button>
    </template>
</Child>
<Child>
    <template v-slot:header>
        <h1>Jay</h1>
    </template>
    <template v-slot:content>
        <p>A Vue Js Product</p>
    </template>
    <template v-slot:footer>
        <button>Click Me</button>
    </template>
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
