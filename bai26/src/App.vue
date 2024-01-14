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
            <p>You can opt out of our newsletters at any time. See our privacy policy</p>
            <div class="input">
              <input type="email" name="email" placeholder="Enter email hear..">
              <button type="button" onclick="alert('Hello I am email')"><i class="fa fa-paper-plane-o"
                  aria-hidden="true"></i></button>
            </div>
          </div>

          <div class="col234">
            <div class="col" v-for="x in col">
              <ul>
                <li v-for="y in x.li"><a v-bind:href="y.link">{{ y.message }}</a></li>
              </ul>
            </div>
          </div>
        </div>

        <div class="foot">

          <div class="border">
            <p>190 x 50</p>
          </div>

          <div class="foot-right">
            <i class="fa fa-copyright" aria-hidden="true"></i>
            <p>Copyright Học Web Chuẩn All Rights Resserved</p>
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
          li: [
            {
              link: '#About us',
              message: 'About us'
            },
            {
              link: '#About me',
              message: 'About me'
            },
            {
              link: '#Our Services',
              message: 'Our Services'
            },
            {
              link: '#Our Team',
              message: 'Our Team'
            },
            {
              link: '#Contact us',
              message: 'Contact us'
            }
          ]

        },
        {
          li: [
            {
              link: '#Get In Touch',
              message: 'Get In Touch'
            },
            {
              link: "#FAQ's",
              message: "FAQ's"
            },
            {
              link: '#Testimonials',
              message: 'Testimonials'
            },
            {
              link: '#Elements',
              message: 'Elements'
            },
            {
              link: '#Not Found',
              message: 'Not Found'
            }
          ]

        },
        {
          li: [
            {
              link: '#Checkout',
              message: 'Checkout'
            },
            {
              link: '#Shopping Cart',
              message: 'Shopping Cart'
            },
            {
              link: '#My Account',
              message: 'My Account'
            },
            {
              link: '#Login / Register',
              message: 'Login / Register'
            }
          ]

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
  width: 85%;
  margin: auto;
  background-color: #000000;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.content {
  color: #757373;
  font-size: 16px;
}

.head {
  display: flex;
  justify-content: space-between;
  padding: 60px 70px 70px;
}

.col1 {
  width: 32%;

}

.col234 {
  display: flex;
  width: 50%;
  justify-content: space-between;
}

.col {
  width: 33%;
}

ul {

  list-style-type: none;
  padding: 0;
  line-height: 38px;
}

a:link,
a:visited {
  text-decoration: none;
  color: #606060;
}

a:hover {
  color: #999898;
}

.input {
  margin-top: 40px;
}

input {
  background-color: #151515;
  border: none;
  height: 45px;
  width: 250px;
  padding: 0 12px;
  color: #999898;
}

button {
  background-color: #01bacf;
  color: white;
  width: 60px;
  height: 45px;
  border: none;

}

button i {
  font-size: 15px !important;
}

.foot {
  background-color: #151515;
  display: flex;
  justify-content: space-between;
  padding: 25px 70px;
}

.border {
  background-color: #8598cc;
  color: white;
  font-size: 25px;
  font-weight: 200;
  width: 190px;
  height: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.foot-right {
  display: flex;
  align-items: baseline;
}

.foot-right i {
  font-size: 15px !important;
}
</style>
