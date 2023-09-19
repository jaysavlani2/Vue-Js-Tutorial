<template>
<h1>Call Get API</h1>
<p v-for="item in list" key="item">
    {{ item.id }} --- {{ item.email }} --- {{ item.first_name }} 
</p>
</template>

<script>
import axios from 'axios';

export default {
    name: 'Home',
    data() {
        return {
            list: []
        }
    },
    async mounted() {
        const res = await axios.get('https://reqres.in/api/users?page=1');
        this.list = res.data.data;
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
