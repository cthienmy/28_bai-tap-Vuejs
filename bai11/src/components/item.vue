<template>
    <div class="item">
        <div class="icon">
            <div class="circle">
                <i v-bind:class="icon" aria-hidden="true"></i>
            </div>
        </div>
        <h2>{{ title }}</h2>
        <p>Lorem ipsum dolor sit amet, consect adipis elit minim veniam ettis inkeras.</p>
    </div>
</template>
<script>
export default {
    props: [
        'icon', 'title'
    ]
}
</script>
<style>
.item {
    background-color: #f8f8f8;
    text-align: center;
    padding: 28px 10px 10px;
    box-sizing: border-box;
}

.icon {
    color: #339999;
    font-size: 30px;
    display: flex;
    justify-content: center;
}

.circle {
    border: 2px solid;
    height: 70px;
    width: 70px;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;

}

p {
    color: #818181;
    font-size: 15px;
    line-height: 23px;
}
</style>