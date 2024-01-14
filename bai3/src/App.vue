<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <div class="container">
    <div>
      <div class="content">
        <h1>Don't miss this special offer!</h1>
        <p>Get it now for just $10! the price will be increased after 50 downloads</p>
      </div>
      <button>Get the latest version of Bootslader</button>
    </div>

  </div>
</template>

<style>
.container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;


}

div div:first-child {
    background-image: url('b4ef9084598789d9d096.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    color: white;
    text-align: center;
    width: 67%;
    object-fit: cover;
    padding: 40px 0 20px 0;

}

.content {
    display: inline;

}

h1 {
    margin-bottom: 30px;
}

button {
    background-color: #e1503b;
    color: white;
    padding: 15px;
    border-radius: 5px;
    font-size: 17px;
    margin: 40px 0;
}
</style>