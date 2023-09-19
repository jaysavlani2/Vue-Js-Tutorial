<template>
<h1>Form Validation</h1>
<ul>
    <li v-for="item in error" :key="item">
        {{ item }} not valid
    </li>
</ul>
<form>
    <label>Email:</label>
    <input type="text" placeholder="Enter email" v-model="form.email" />
    <br /><br />
    <label>Password:</label>
    <input type="password" placeholder="Enter password" v-model="form.password" />
    <br /><br />

    <label>Country:</label>
    <select v-model="form.country">
        <option value="India">India</option>
        <option value="England">England</option>
        <option value="Australia">Australia</option>
    </select>
    <br /><br />

    <h3>Technology:</h3>
    <label>React:</label>
    <input type="checkbox" v-model="form.technology" value="react" />
    <br /><br />
    <label>Vue:</label>
    <input type="checkbox" v-model="form.technology" value="vue" />
    <br /><br />

    <h3>Gender:</h3>
    <label>Male:</label>
    <input type="radio" v-model="form.gender" value="Male" name="gender" />
    <br /><br />
    <label>Female:</label>
    <input type="radio" v-model="form.gender" value="Female" name="gender" />
    <br /><br />

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
                country: '',
                technology: [],
                gender: '',
            },
            error: []
        }
    },
    methods: {
        login() {
            this.error = []
            for (const item in this.form) {
                if (this.form[item] === "" || this.form[item].length === 0) {
                    this.error.push(item)
                }
            }
            if(this.error.length === 0){
                alert('Form submitted')
            }
            console.log('Login Data:', this.form, this.error)
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
