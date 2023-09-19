<template>
<h1>Teleport Component</h1>
<teleport to="#footer">
    <Footer></Footer>
</teleport>
</template>

<script>
import Footer from './Footer.vue';
export default {
    name: 'Home',
    components: {
        Footer
    },
    data() {
        return {

        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
