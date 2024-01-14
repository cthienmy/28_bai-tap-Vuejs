<!-- <script setup> 
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script> -->

<template>
  <div class="container1">
    <div class="container2">

      <div class="border">
        <p>Học Web Chuẩn</p>
      </div>

      <div class="content">

        <div class="head">
          <h1>ABOUT US</h1>
          <div></div>
        </div>

        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore
          magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
          consequat. Lorem ipwum dolor sit amet, consectetur adipiscing elit, quis nostrud exercitation ullamco laboris
          nisi ut aliquip ex ea commodo consequat. </p>

        <div class="foot">
          <h2>Why Choose Us</h2>

          <div class="list">

            <div class="col" v-for="x in col">
              <ul>
                <li v-for="y in x.lii">
                  <i class="fa fa-check" aria-hidden="true"></i>
                  <a v-bind:href="y.link">{{ y.message }} </a>
                </li>
              </ul>
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
          lii: [
            { link: '#Lorem ipsum dolor', message: 'Lorem ipsum dolor' },
            { link: '#Tempor incididunt', message: 'Tempor incididunt' },
            { link: '#Lorem ipsum dolor', message: 'Lorem ipsum dolor' },
            { link: '#Incididunt ut labore', message: 'Incididunt ut labore' }
          ]
        },
        {
          lii: [
            { link: '#Aliquip ex ea commodo', message: 'Aliquip ex ea commodo' },
            { link: '#Lorem ipsum dolor', message: 'Lorem ipsum dolor' },
            { link: '#Exercitation ullamco', message: 'Exercitation ullamco' },
            { link: '#Lorem ipsum dolor', message: 'Lorem ipsum dolor' }
          ]
        }
      ]
    }
  }
}
</script>

<style >
.container1 {
  padding: 100px 0;
}

.container2 {
  width: 80%;
  margin: auto;
  display: flex;
  justify-content: space-between;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.border {
  width: 45%;
  background-color: #2e2e2e;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 50px;
  font-weight: 100;
}

.content {
  width: 48%;
  color: #8a8a8a;
  line-height: 25px;
}

h1,
h2 {
  color: #333333;
}

h2 {
  font-weight: 500;
  margin: 30px 0 5px;
}

.head {
  margin: 35px 0;
}

.head div {
  border-top: 5px solid #627bfe;
  width: 60px;
}

.foot {}

.list {
  display: flex;
  justify-content: space-between;
  padding: 0;
}

.col {}

ul {
  list-style-type: none;
  padding: 0 0 0 20px;
}

li {}

i {
  color: #5fabfb;
  margin-right: 5px;
  font-size: 12px !important;
}

a:link,
a:visited {
  text-decoration: none;
  color: #a6a6a6;
}
</style>
