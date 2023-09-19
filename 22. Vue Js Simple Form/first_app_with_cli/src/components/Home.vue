<template>
<h1>Simple Form</h1>
<p>{{ form }}</p>
<form>
    <label>Email:</label>
    <input type="text" placeholder="Enter email" v-model="form.email"/><br /><br />
    <label>Password:</label>
    <input type="password" placeholder="Enter password" v-model="form.password"/><br /><br />
    <button type="button" v-on:click="login()">Submit</button>
</form>
</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
            form: {
                email: '',
                password: '',
            }
        }
    },
    methods: {
        login() {
            console.log('Login Data:', this.form)
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
