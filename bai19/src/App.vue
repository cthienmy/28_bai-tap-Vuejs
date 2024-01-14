<!-- <script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script> -->

<template>
  <div class="container">
    <div class="background">

      <div class="head">

        <h1>Issues & Plans</h1>
        <p>Quisque eget nisl id nulla sagittis auctor quis is. Aliquam quis vehicula enim, non aliquam risus.<br> Sed a
          tellus quis mi rhoncus dignissim.</p>

      </div>

      <div class="foot">

        <div class="col1">

          <div class="image">
            <p>Học Web Chuẩn</p>
          </div>

          <div class="image-foot">
            <h2>"Turkey Will Continue To Make Structural Economic Reforms"</h2>
            <p>Etiam materials ut mollis tellus, vel posuere nulla. Etiam sit amet massa sodales aliquam at eget quam.
              Integer ultricies et magna quis.</p>
            <p>Tiam sit amet lacus vitae massa sodales aliquam at eget quam.
              Integer ultricies et magna quis.
            </p>
          </div>

        </div>

        <div class="col2">

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
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  line-height: 26px;
}

.background {
  width: 80%;
  margin: auto;
  background-color: #f2f3f5;
  padding: 10px 30px;
  color: #a6a6a7;
}

h1,
h2,
h3 {
  color: #424243;
}


.head {}

.head h1 {
  font-size: 40px;
}

.head p {
  font-size: 20px;
  line-height: 32px;
  margin: 40px 0;
}

.foot {
  display: flex;
}


.col1 {
  width: 40%;
  padding: 20px 30px 10px 0;
}

.image {
  background-color: #789ade;
  color: white;
  height: 320px;
  border-radius: 5px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 45px;
  font-weight: 300;
}

.image-foot {}



.col2 {
  width: 60%;
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

}

h3 {
  margin: 0;
  font-weight: 500;
}

.item p {

  margin: 12px 0;
}</style>
