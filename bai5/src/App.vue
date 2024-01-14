<script setup>
import boA from './components/border.vue'
import boB from './components/paragraphs.vue'
</script>

<template>
  <div class="container">
      <div class="content">

        <boA/>

        <boB/>

      </div>
    </div>
</template>

<style>
.container{
display: flex;
justify-content: center;
font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
padding-top: 80px;
}

.content{
    display:inline-flex;
    width: 70%;
}






</style>
