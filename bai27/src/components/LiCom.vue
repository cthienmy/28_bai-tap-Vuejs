<template >
    <li>
        <i class="fa fa-check" aria-hidden="true"></i>
        <a v-bind:href="link">{{ message }}</a>
    </li>
</template>
<script>
export default {
    props: ["message", "link"]
}
</script>
<style lang="">
    
</style>