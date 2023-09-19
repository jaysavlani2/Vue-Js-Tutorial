<template>
    <div>
        <h2>Jay</h2>
        <h2>ABC</h2>
        <h2>XYZ</h2>
        <h2>{{ data }}</h2>
        <h2 v-bind="$attrs">QWERTY</h2>
    </div>
</template>

<script>
export default {
    name: 'User',
    props: {
        data: String
    },
    inheritAttrs: false
}
</script>