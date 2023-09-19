<template>
<h1>Dynamic Component</h1>
<button @click="tab='React'">Load React</button>
<button @click="tab='Vue'">Load Vue</button>
<button @click="tab='Node'">Load Node</button>
<component :is="tab"/>
</template>

<script>
import React from './React.vue';
import Node from './Node.vue';
import Vue from './Vue.vue';
export default {
    name: 'Home',
    components: {
        React,
        Node,
        Vue
    },
    data() {
        return {
            tab: 'React'
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
