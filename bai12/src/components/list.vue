<template>
    <li><a v-bind:href="link">{{message}}</a></li>
</template>
<script>
export default {
       props: [
        'link', 'message'
       ]
}
</script>
<style scoped>
a:link, a:visited {
    text-decoration: none;
    color: rgb(60, 60, 60);
    padding: 15px;
}

a:hover,
a:active {
    color: #2dbcf2;
}
</style>