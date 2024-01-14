<template>
    <h3>{{ title }}</h3>
</template>
<script>
export default {
    props: [
        'title'
    ]
}
</script>
<style scoped>
    h3{
    font-weight:500;
    margin-bottom: 35px;
    color:#393939;
}
</style>