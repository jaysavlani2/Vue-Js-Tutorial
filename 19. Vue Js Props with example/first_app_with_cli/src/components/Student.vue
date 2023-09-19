<template>
<h2>Student Data: {{ name }}</h2>
</template>

<script>
export default {
    name: 'Student',
    props: {
        name: String
    }
}
</script>
