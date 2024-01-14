<script setup>
import itE from './components/item.vue'

</script>

<template>
  <div class="container">
    <div class="content">

      <itE icon="fa fa-leaf" title="UI/UX Design" />
      <itE icon="fa fa-desktop" title="Web Development" />
      <itE icon="fa fa-briefcase" title="Branding" />
      <itE icon="fa fa-camera" title="Photography" />
      <itE icon="fa fa-android" title="Apps Development" />
      <itE icon="fa fa-line-chart" title="Digital Marketing" />


    </div>
  </div>
</template>

<style>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  font-family: Arial, Helvetica, sans-serif;

}

.content {
  width: 80%;
  display: grid;
  grid-template-columns: auto auto auto;
  gap: 30px;
}
</style>
