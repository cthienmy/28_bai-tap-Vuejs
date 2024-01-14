<template>
    <li><a v-bind:href="link">{{ message }}</a></li>
</template>
<script>
export default {
    props: [
        'link', 'message'
    ]
}
</script>
<style scoped>
a:link,
a:visited {
    text-decoration: none;
    color: #bababa;
    letter-spacing: 1px;

}

a:hover,
a:active {
    color: #99d9df;
}
</style>