<template>
<h1>HTML Binding</h1>
<h2>{{ text }}</h2>
<div v-html="tag"></div>
<div v-html="tag2"></div>
<div v-html="tag + tag2 + tag3"></div>
</template>

<script>
export default {
    name: 'Home',
    data(){
        return {
            text: 'Jay Savlani',
            tag: '<h2>Jay Savlani</h2>',
            tag2: '<h2>jay@gmail.com</h2>',
            tag3: '<h2>test@gmail.com</h2>',
        }
    },
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
