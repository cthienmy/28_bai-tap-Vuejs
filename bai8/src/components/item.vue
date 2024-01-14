<template>
    <div class="item">
        <div>
            <div class="HWC">
                <p>HWC</p>
            </div>
        </div>
        <div class="vb">
            <p>{{ message }}</p>
        </div>
    </div>
</template>
<script>
export default {
    props: [
        'message'
    ]
}
</script>
<style scoped>
.item {}

.item div {
    display: flex;
    justify-content: center;
}

.HWC {
    border: none;
    background-color: #cc784e;
    width: 45px;
    height: 45px;
    color: white;
    font-size: 11px;
    font-weight: 200;
    display: flex;
    justify-content: center;
    align-items: center;
}

.vb {
    font-weight: 600;
    font-size: 17px;
}
</style>