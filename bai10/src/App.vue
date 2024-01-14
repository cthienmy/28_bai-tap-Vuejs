<script setup>
import itE from './components/item.vue'

</script>

<template>
  <div class="container">
    <div class="content">

      <itE icon="fa fa-globe" number="3297" message="Foreign Followers" />
      <itE icon="fa fa-graduation-cap" number="3700" message="Students Enrolled" />
      <itE icon="fa fa-lightbulb-o" number="5034" message="Classes Complete" />
      <itE icon="fa fa-user-o" number="1080" message="Certified Teachers" />

    </div>
  </div>
</template>

<style>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  font-family: 'Times New Roman', Times, serif;
}

.content {
  width: 80%;
  background-image: url('b4ef9084598789d9d096.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  justify-content: space-around;
  color: rgb(224, 224, 224);
  padding: 35px 90px;
  box-sizing: border-box;
}
</style>
