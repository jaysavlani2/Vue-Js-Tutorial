<template>
    <h1>Get CHeckbox & Radio Button Value</h1>
    <h3>Technologies</h3>
    <label for="react">React</label>
    <input type="checkbox" value="React" id="react" v-model="technologies"/> &nbsp;
    <label for="node">Node</label>
    <input type="checkbox" value="Node" id="node" v-model="technologies"/>&nbsp;
    <label for="vue">Vue</label>
    <input type="checkbox" value="Vue" id="vue" v-model="technologies"/>
    <h4>Selected Technology: {{ technologies }}</h4>

    <br/><br/>

    <h3>Who I am? {{ who }}</h3>
    <label for="student">Student</label>
    <input type="radio" value="Student" id="student" name="who" v-model="who"/> &nbsp;
    <label for="developer">Developer</label>
    <input type="radio" value="Developer" id="developer" name="who" v-model="who"/>
</template>

<script>
export default {
    name:'Home',
    data(){
        return {
            technologies:[],
            who: null
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>