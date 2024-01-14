<!-- <script setup>
//import HelloWorld from './components/HelloWorld.vue'
//import TheWelcome from './components/TheWelcome.vue'
</script> -->

<template>
  <div class="container">

    <div class="background">
      <div class="content">

        <div class="head">
          <h1>Our Service</h1>
          <p>Our Service unlimited solutions to all your business needs, in the installation packge we prepare search
            engine optimization, social media supprt, we provide corporate identily and graphic design services.</p>
        </div>

        <div class="border">

          <div class="col" v-for="x in col">
            <div class="image">
              <p>Học Web Chuẩn</p>
            </div>
            <div class="item" >
              <h2>{{ x.item.title }}</h2>
              <p>{{ x.item.message }}</p>
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
      col: [
        {
          item:
            { title: 'Smart Swatch Editions', message: 'Aliquam sagittis ligula et sem lacinia, ut facilisis enim sollicitudin. Proin nisi est, convallis nec purus vitae, iaculis posuere sapien. Cum sociis natoque, ut facilisis.' }
        },
        {
          item:
            { title: 'Web UI Kit Design', message: 'Duis at tellus at dui tincidunt sceletisque nec sed felis. Suspendisse id dolor sed leo rutrum euismod. Nullam vestibulum fermentm erat. It nam auctor.' }
        },
        {
          item:
            { title: 'Mobile Optimization', message: 'Etiam materials ut mollis tellus, vel posuere nulla. Etiam sit amet lacus vitae massa sodales aliquam at eget quam. Integer ultricies et magna quis accumsan.' }
        }
      ]
    }
  }
}
</script>

<style>
.container {
  padding: 40px 0;
}

.background {
  width: 82%;
  margin: auto;
  background-color: #f2f3f5;
  padding: 30px 15px 50px;
}

.content {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  color: #b3b3b4;

}

.head {
  text-align: center;
  font-size: 20px;
  padding: 0 40px 40px;
  line-height: 30px;

}



h1 {
  color: rgb(57, 56, 56);
  font-weight: 400;
  font-size: 42px;
  padding-bottom: 15px;

}

h2 {
  color: rgb(75, 74, 74);
  font-weight: 500;
  margin: 0 0 10px 0;
}

.border {
  display: grid;
  grid-template-columns: 30% 30% 30%;
  justify-content: space-evenly;
}

.col {}

.image {
  background-color: #91e0e6;
  color: #ffffff;
  display: flex;
  justify-content: center;
  height: 220px;
  align-items: center;
  font-size: 30px;
  font-weight: 100;
}

.item {
  background-color: white;
  padding: 30px 15px 20px;
  line-height: 25px;
}

.item p {
  margin: 0;
}
</style>
