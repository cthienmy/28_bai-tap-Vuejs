<template>
    <div class="item">
        <i v-bind:class= "icon"  aria-hidden="true"></i>
        <p>{{ number }}</p>
        <p>{{ message }}</p>
    </div>
</template>
<script>
export default {
   props:[
    'icon','number', 'message'
   ]
}
</script>
<style scoped>
.item {
    text-align: center;
    font-size: 50px;
}

.item p:nth-child(2) {
    margin: 15px 0 20px 0;
    font-size: 50px;

}

.item p:nth-child(3) {
    margin: 0;
    font-size: 20px;
}
</style>