<script setup>
import toH from './components/head.vue'
import toN from './components/navbar.vue'
import botB from './components/border.vue'
</script>

<template>
  <div class="container">
    <div class="content">

      <div class="top">

        <toH />

        <toN />

      </div>

      <div class="bottom">
        <botB />
      </div>


    </div>
  </div>
</template>

<style>
.container {
  display: flex;
  justify-content: center;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.content {
  width: 80%;
  text-align: center;
  background-color: #f8f8f8;
  margin: 40px 0;
}

.top {}







.bottom {
  background-color: white;
  margin: 20px 15px;


}
</style>
