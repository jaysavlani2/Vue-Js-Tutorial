<template>
<h1>User Component</h1>
<button v-on:click="getUserName(userName)">Send User Name</button>
</template>

<script>
export default {
    name: 'User',
    data() {
        return {
            userName: 'Jay' 
        }
    },
    props: {
        getUserName: Function
    }
}
</script>
