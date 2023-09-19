<template>
<h1>Reuse Component</h1>
<ul>
    <li v-for="item in users" :key="item.name">
        <User :item="item" :getData="getData"/>
    </li>
</ul>
</template>

<script>
import User from './User.vue';
export default {
    name: 'Home',
    components: {
        User
    },
    data() {
        return {
            users: [{
                    name: 'Jay',
                    email: 'jay.savlani2@gmail.com'
                },
                {
                    name: 'Ayush',
                    email: 'ayush@gmail.com'
                },
                {
                    name: 'Xyz',
                    email: 'xyz@gmail.com'
                },
                {
                    name: 'Sam',
                    email: 'sam@gmail.com'
                },
            ]
        }
    },
    methods: {
        getData(item){
            console.log(item)
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
