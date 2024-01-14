<script setup>
import liA from './components/list.vue'

</script>

<template>
  <div class="container">
    <div class="content">

      <div class="item1">
        <div class="border">
          <p>190 x 50</p>
        </div>

        <div class="navbar">
          <ul>
            <liA link="#Home" message="Home" />
            <liA link="#Features" message="Features" />
            <liA link="#Domain" message="Domain" />
            <liA link="#Hosting" message="Hosting" />
            <liA link="#Pricing" message="Pricing" />
            <liA link="#Testimonials" message="Testimonials" />
            <liA link="#Contact" message="Contact" />


          </ul>
        </div>

      </div>

      <div class="login">
        <button>
          <i class="fa fa-unlock-alt" aria-hidden="true"></i>
          <p>Customer Login</p>
        </button>
      </div>


    </div>
  </div>
</template>

<style>
.container {
  padding-top: 100px;
}

.content {
  width: 78%;
  display: flex;
  justify-content: space-between;
  margin: auto;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.item1 {
  display: flex;
}

.border {
  background-color: #8598cc;
  width: 190px;
  height: 50px;
  color: white;
  font-size: 20px;
  display: flex;
  justify-content: center;
  align-items: center;

}

.border p {
  font-weight: lighter;
  margin: 0;
}

.navbar {}

ul {
  display: flex;
  list-style-type: none;
  padding: 0 0 0 15px;
}



.login {
  display: flex;
  align-items: center;
}

button {
  display: flex;
  align-items: center;
  border: 3px solid #efefef;
  border-radius: 4px;
  padding: 12px 15px;
  background-color: white;
  font-size: 15px;
  cursor: pointer;
  color: rgb(60, 60, 60);
}

button:hover {
  background-color: rgb(250, 249, 249);
}

button p {
  padding-left: 7px;
  margin: 0;
}
</style>
