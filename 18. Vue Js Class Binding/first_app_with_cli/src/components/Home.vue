<template>
<h1>Class Binding</h1>
<h2 :class="applyStyle">Home Component</h2>
<button v-on:click="color=!color">Click</button>
</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
            color: true
        }
    },
    computed:{
        applyStyle(){
            return {
                green: this.color,
                red: !this.color,
                other: true
            }
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
.green{
    background-color: green;
    width: 400px;
    padding: 10px;
}
.red{
    background-color: red;
    width: 400px;
    padding: 10px;
}
.other {
    font-size: 50px;
}
</style>
