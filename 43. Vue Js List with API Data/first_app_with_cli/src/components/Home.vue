<template>
<h1>Call Get API</h1>
<ul class="item" v-for="item in list" :key="item.id">
    <li>
        {{ item.id }}
    </li>
    <li>
        {{ item.email }}
    </li>
    <li>
        {{ item.first_name }}
    </li>
    <li>
        <img :src="item.avatar" :alt="item.id"/>
    </li>
</ul>
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

.item {
    display: flex;
}

.item li {
    display: inline-block;
    width: 200px;
    border: 1px solid red;
    padding: 5px;
}
</style>
