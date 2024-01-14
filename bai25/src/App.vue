<!-- <script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script> -->

<template>
  <div class="container">
    <div class="background">
      <div class="background-top"></div>
      <div class="background-bottom"></div>

      <div class="content">

        <div class="head">
          <h1>Hello, we have brought together the best quality services, offers, projects for you!</h1>
        </div>

        <div class="border">

          <div class="item" v-for="x in item">
            <div class="icon"><i v-bind:class="x.icon" aria-hidden="true"></i></div>
            <div class="item-content">
              <h2>{{ x.itemcontent.h2 }}</h2>
              <p>{{ x.itemcontent.message }}</p>
            </div>
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
      item: [
        {
          icon: 'fa fa-desktop',
          itemcontent: {
            h2: 'Outstanding design',
            message: 'Designed to be flexible according to all your neesd. Create your dite with all module position.'
          }

        },
        {
          icon: 'fa fa-mobile',
          itemcontent: {
            h2: 'Responsive Layout',
            message: 'Genius template can be easily viewed on any mobile device. Smoothly responsive.'
          }

        },
        {
          icon: 'fa fa-cogs',
          itemcontent: {
            h2: 'Easy to use',
            message: 'The modules we have prepared are simple to use. No code information is needed.'
          }

        }
      ]
    }
  }
}
</script>

<style>
.container {}

.background {
  width: 90%;
  margin: auto;
  position: relative;

}

.background-top {
  background-color: #01bacf;
  height: 230px;
}

.background-bottom {
  background-color: #f7f6f6;
  height: 400px;
}

.content {
  height: 630px;
  position: absolute;
  top: 0;
  bottom: 0;

  padding: 50px 90px;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.head {}

.head h1 {
  margin: 0 200px 50px 0;
  color: white;
  font-size: 35px;
  font-weight: 500;
}

.border {
  display: flex;
  justify-content: space-between;

}

.item {
  width: 31.5%;
  background-color: white;
  padding: 50px 30px;
  box-sizing: border-box;
}

.icon {}

i {
  color: #c2d82e;
  font-size: 43px !important;
}

.item-content {}

.item-content h2 {
  font-weight: 500;
}

.item-content p {
  color: #a2a1a1;
  font-size: 17px;
  line-height: 25px;

}
</style>
