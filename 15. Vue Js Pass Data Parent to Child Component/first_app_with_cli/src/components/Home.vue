<template>
<h1>Pass Data Parent to Child Component</h1>
<Child name="Jay Savlani" :user="user" :getData="getData"/>
</template>

<script>
import Child from './Child.vue'
export default {
    name: 'Home',
    components: {
        Child
    },
    data(){
        return {
            user: {
                email: 'Jaysavlani2@gmail.com',
                name: 'Jay Savlani'
            }
        }
    },
    methods: {
        getData(){
            console.log('Hii')
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
