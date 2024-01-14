<script setup>
import heD from './components/head.vue'
import itE from './components/item.vue'
</script>

<template>
  <div class="container">
    <div class="content">

      <heD />

      <div class="border">

        <itE message="We plan properly"/>
        <itE message="We start project"/>
        <itE message="We showcase work"/>
        <itE message="You'll be happy"/>



      </div>
    </div>
  </div>
</template>

<style>
.container {
  display: flex;
  justify-content: center;
  height: 100vh;
  align-items: center;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.content {
  width: 70%;
}



.border {
  display: flex;
  justify-content: space-between;

}
</style>
