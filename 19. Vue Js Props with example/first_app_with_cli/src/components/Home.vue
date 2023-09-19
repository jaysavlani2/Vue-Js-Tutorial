<template>
<h1>Props</h1>
<Student :name="name"/>
<Teacher :name="name"/>
</template>

<script>
import Student from './Student.vue';
import Teacher from './Teacher.vue';
export default {
    name: 'Home',
    data(){
        return {
            name: 'Jay'
        }
    },
    components: {
        Student,
        Teacher
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
