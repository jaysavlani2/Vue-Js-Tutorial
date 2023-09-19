<template>
<h1>For Loop in Vue Js</h1>
<ul>
    <li v-for="item in technology" :key="item">
        {{ item }}
    </li>
</ul><br/>
<ul>
    <li v-for="item in user" :key="item">
        Name: {{ item.name }} and Email : {{ item.email }}
    </li>
</ul>
</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
            technology: ['React', 'Node', 'JavaScript', 'Vue'],
            user: [{
                    name: 'Jay',
                    email: 'jay@test.com'
                },
                {
                    name: 'Prince',
                    email: 'prince@test.com'
                },
                {
                    name: 'Sam',
                    email: 'sam@test.com'
                }
            ]
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
