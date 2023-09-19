<template>
<h1>Post Method API</h1>
<input type="text" name="email" v-model="email" /> <br />
<input type="password" name="password" v-model="password" /> <br />
<button type="button" v-on:click="submitData()">Submit</button>
</template>

<script>
import axios from 'axios';

export default {
    name: 'Home',
    data() {
        return {
            email: '',
            password: '',
        }
    },
    methods: {
        async submitData() {
            const result = await axios.post('', {
                email: this.email,
                password: this.password
            })
            console.log(result)
        }
    }
}
</script>
