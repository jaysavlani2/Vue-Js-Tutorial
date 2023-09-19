<template>
    <h1>Email: {{ email }}</h1>
    <h1>Mobile: {{ mobile }}</h1>
    <h1>Name: {{ getName('Jay') }}</h1>
    <h1>Value: {{ value }}</h1>
    <h1>Value: {{ value=9999 }}</h1>
</template>

<script>
export default {
    name:'Home',
    data(){
        return {
            email: 'jaysavlani2@gmail.com',
            mobile: '928292',
            getName: function(name){
                return name
            },
            value: 8888,
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>