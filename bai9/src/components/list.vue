<template>
    <a v-bind:href="link">
        <li>{{ message }}</li>
    </a>
</template>
<script>
export default {
    props: [
        'message', 'link'
    ]
}
</script>
<style>
li {
    background-color: #01bacf;
    padding: 6px 10px;
    margin: 5px 7px;
    border-radius: 3px;

}

a {
    text-decoration: none;
    color: white;

}
</style>