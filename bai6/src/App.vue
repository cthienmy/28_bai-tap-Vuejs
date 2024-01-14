<script setup>
import hedA from './components/head.vue'
import boB from './components/border.vue'
</script>

<template>
  <div class="container">
    <div class="content">

      <hedA />

      <boB />

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
  width: 65%;
}
</style>
