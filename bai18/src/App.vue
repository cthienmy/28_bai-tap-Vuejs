<!-- <script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script> -->

<template>
  <div class="container">
    <div class="background">
      <div class="content">

        <div class="row" v-for="x in row">
          <div class="border">
            <P>H</P>
          </div>

          <div class="item">
            <h3>{{ x.item.title }}</h3>
            <p>{{ x.item.message }}</p>
          </div>
        </div>



      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      row: [
        {
          item: {
            title: 'CLIMATE CHANGE',
            message: 'Etiam materials ut mollis tellus, vel posuere nulla. Etiam sit amet lacus vitae massa sodales aliquam at eget quam. Integer ultricies et magna quis.'
          }
        },
        {
          item: {
            title: 'COMPREHENSIVE IMMIGRATION REFORM',
            message: 'Etiam materials ut mollis tellus, vel posuere nulla. Etiam sit amet lacus vitae massa sodales aliquam at eget quam. Integer ultricies et magna quis.'
          }
        },
        {
          item: {
            title: 'ECONOMIC OPPORTUNITY',
            message: 'Etiam materials ut mollis tellus, vel posuere nulla. Etiam sit amet lacus vitae massa sodales aliquam at eget quam. Integer ultricies et magna quis.'
          }
        },
        {
          item: {
            title: 'HEALTH CARE',
            message: 'Etiam materials ut mollis tellus, vel posuere nulla. Etiam sit amet lacus vitae massa sodales aliquam at eget quam. Integer ultricies et magna quis.'
          }
        }
      ]
    }
  }
}
</script>

<style>
.container {
  padding: 50px 0;
}

.background {
  width: 45%;
  margin: auto;
  background-color: #f2f3f5;
  padding: 10px 25px;
}

.content {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.row {
  display: flex;
  padding: 20px 0;
  border-bottom: 2px dashed #f3928c;
}

.row:nth-child(4) {
  border: none;
}

.border {
  width: 15%;
  background-color: #d997de;
  color: white;
  font-size: 70px;
  font-weight: 200;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 6px;
}

.border p {
  margin: 0;
}

.item {
  width: 85%;
  padding-left: 30px;
  color: #a6a6a7;
}

h3 {
  margin: 0;
  font-weight: 500;
  color: #424243;
}

.item p {
  line-height: 26px;
  margin: 12px 0;
}
</style>
