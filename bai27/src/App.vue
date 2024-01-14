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

      <div class="col">
        <div class="content">

          <h1>We are a passionte <span>&nbsp;Iearning system&nbsp;</span> from London. Do beautiful and easy-to-use
            digital design & web development</h1>
          <p>Nam dictum sem, ipsum aliquam. Etiam sit amet fringilla lacus. Pellentesque suscipit ante at ullamcorper
            pulvinar neque porttitor. Integer lectus. Praesent sed nisi eleifend, fermentum orci amet, iaculis libero.</p>

          <div class="list">
            <div class="list-col" v-for="x in listcol">
              <ul>
                <!-- <li v-for="y in x.li">
                  <i class="fa fa-check" aria-hidden="true"></i>
                  <a v-bind:href="y.link">{{ y.message }}</a>
                </li> -->

                <LiCom v-for="y in x.li" v-bind:message="y.message" v-bind:link="y.link" />
              </ul>
            </div>
          </div>
          <button>Learn More Abaout Us</button>
        </div>
      </div>

    </div>
  </div>
</template>

<script>
import LiCom from "./components/LiCom.vue"
export default {
  components: {
    LiCom
  },
  data() {
    return {
      listcol: [
        {
          li: [
            {

              link: '#Custom Shortcodes',
              message: 'Custom Shortcodes'
            },
            {

              link: '#Visual Page Builder',
              message: 'Visual Page Builder'
            },
            {

              link: '#Unlimited Shortcodes',
              message: 'Unlimited Shortcodes'
            },
            {

              link: '#Responsive Theme',
              message: 'Responsive Theme'
            },
            {

              link: '#Tons of Layouts',
              message: 'Tons of Layouts'
            }
          ]
        },
        {
          li: [
            {

              link: '#Font Awesome Icons',
              message: 'Font Awesome Icons'
            },
            {

              link: '#Pre-Defined Colors',
              message: 'Pre-Defined Colors'
            },
            {

              link: '#AJAX Transitions',
              message: 'AJAX Transitions'
            },
            {

              link: '#High Quality Support',
              message: 'High Quality Support'
            },
            {

              link: '#Unlimited Options',
              message: 'Unlimited Options'
            }
          ]
        },
        {
          li: [
            {

              link: '#Shopping Layouts',
              message: 'Shopping Layouts'
            },
            {

              link: '#Pre-Defined Fonts',
              message: 'Pre-Defined Fonts'
            },
            {

              link: '#Style Changers',
              message: 'Style Changers'
            },
            {

              link: '#Footer Styles',
              message: 'Footer Styles'
            },
            {

              link: '#Header Styles',
              message: 'Header Styles'
            }
          ]
        }
      ]
    }
  }
}
</script>

<style>
.container1 {}

.container2 {
  width: 79%;
  margin: auto;
  display: flex;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.border {
  background-color: #66d469;
  width: 33%;
  color: white;
  font-size: 32px;
  font-weight: 200;
  display: flex;
  justify-content: center;
  align-items: center;

}

.col {
  width: 67%;
  padding: 0 0 0 70px;
}

.content {
  color: #898787;
  font-size: 17px;
  line-height: 28px;
}

.content h1 {
  color: rgb(40, 39, 39);
  line-height: 45px;
  font-size: 32px;
  font-weight: 600;
  margin-bottom: 32px;
  padding-right: 100px;
}

.content span {
  background-color: #02bacf;
  color: white;

}

.list {
  display: flex;
  justify-content: space-between;
  margin: 50px 60px 50px 0;

}

.list-col {}

ul {
  list-style-type: none;
  padding: 0;
}

i {
  color: #02bacf;
  font-size: 14px !important;
  margin-right: 6px;
}

a:link,
a:visited {
  text-decoration: none;
  color: #989797;
}

a:hover {
  color: #5b5a5a;
}

button {
  background-color: #02bacf;
  color: white;
  border: none;
  padding: 15px 30px;
  font-size: 15px;
}
</style>
