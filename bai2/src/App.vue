<script setup>
import comA from './components/a.vue'
import comB from './components/b.vue'
import comC from './components/c.vue'
</script>

<template>
  <div class="body">
    <div class="head">
        
        <comA/>
        
        <comB/>

        <comC/>

    </div>
  </div>

</template>

<style>
.body{
    text-align: center;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
    margin: 0;
}
.head{
   
}

.text{
    color:white;
    font-size: 20px;
  
}

.second{
margin: 50px;
color: #2d3032;
}

h1 {
    font-size: 45px;
}
span {
    color:#00aeef;
}
p {
     font-size: 20px;
}
.third{

}
button{
    background-color: #2d3032;
    color: white;
    width: 190px;
    height: 50px;
    font-size: 15px;
    border-radius: 4px;
    margin: 0 10px;
}
</style>
