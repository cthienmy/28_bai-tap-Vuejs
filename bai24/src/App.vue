<!-- <script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script> -->

<template>
  <div class="container">
    <div class="background">

      <div class="content">

        <div class="head">
          <div class="col1">
            <h2>About Us</h2>
            <p>Praesent convallis tortor et enim laoreet, vel consectetur purus latoque penatibus et dis parturient.</p>
          </div>


          <div class="col2">
            <h2>{{ col2.title2 }}</h2>
            <ul>
              <li v-for="x in col2.ul2"><a v-bind:href="x.link2">{{ x.message2 }}</a></li>

            </ul>
          </div>

  

          <div class="col3">
            <h2>{{ col3.title3 }}</h2>
            <div class="icon">
              <a v-for="y in col3.arr" v-bind:href="y.href">
                <div v-bind:class="y.class"><i v-bind:class="y.icon" aria-hidden="true"></i></div>
              </a>
             
            </div>
          </div>

        </div>

        <div class="foot">
          <p>Copyright Hoc Web Chuan All Right Reserved</p>
        </div>

      </div>

    </div>
  </div>
</template>

<script>
export default {
  data() {
    const data = {
      col2: {
        title2: 'Quick Links',
        ul2: [
          {
            link2: '#Home',
            message2: 'Home'
          },
          {
            link2: '#Service',
            message2: 'Service'
          },
          {
            link2: '#Appointment',
            message2: 'Appointment'
          }
        ]
      },
      col3: {
        title3:'Follow us',
        arr: [
          {
            href: "#face",
            class: "face",
            icon: "fa fa-facebook"
          },
          {
            href: "#google",
            class: "google",
            icon: "fa fa-google-plus"
          },
          {
            href: "#in",
            class: "in",
            icon: "fa fa-linkedin"
          },
          {
            href: "#twitter",
            class: "twitter",
            icon: "fa fa-twitter"
          }
        ]
      }
    }
    return data;
  }
 
}
</script>

<style>
.container {
  padding-top: 100px;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.background {
  width: 80%;
  margin: auto;
  background-color: #325c6a;
}

.content {
  color: white;
}

.head {
  display: flex;
  justify-content: center;
  padding: 30px 0;
  font-size: 17px;
}

h2 {
  font-weight: 400;
  font-size: 20px;
  margin-bottom: 35px;
}

.col1,
.col2,
.col3 {
  width: 28%;
  box-sizing: border-box;
}

.col2,
.col3 {
  padding-left: 50px;
}

.col3 h2 {
  padding-left: 20px;
}

ul {
  padding-left: 55px;
}

a {
  text-decoration: none;
  color: white;
}

.col3 {
  position: relative;
}

.icon {
  display: flex;
  justify-content: end;
  position: absolute;
  bottom: 1em;
  right: 0;
}

.face,
.google,
.in,
.twitter {
  width: 50px;
  height: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-left: 5px;
}

.face {
  background-color: #3498db;
}

.google {
  background-color: #e74c3c;
}

.in {
  background-color: #2c3e50;
}

.twitter {
  background-color: #3498db;
}


.foot {
  text-align: center;
  border-top: 1px solid #476d79;
  padding: 50px 0;
}

.foot p {
  margin: 0;
}
</style>
