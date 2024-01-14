<script setup>
import col14 from './components/col14.vue'
import TheWelcome from './components/TheWelcome.vue'
</script> 

<template>
  <div class="container1">
    <div class="container2">

      <div class="content">

        <div class="col1">
          <h1>A Elegant Design</h1>
          <p>Bacon ipsum dolor sit amet meatball shank park chop capicola fatback park loin sirloin flank.
            <b>Andouille</b> tongue corned beef rump pork loin shnk meatball capicola turducken venison shankle kevin
            pancetta tri-tip boudin.</p>
          <button>BLUE BUTTON WITH MODAL VIDEO</button>
        </div>

        <div class="col2">
          <img src="ddt.png">
        </div>

      </div>

      <div class="line"></div>

      <div class="content">

        <div class="col3">
          <img src="anh.png">
        </div>

        <div class="col4">
          <h1>Pretty easy to customize</h1>
          <p>Bacon ipsum dolor sit amet meatball shank park chop capicola fatback park loin sirloin flank.<b>
              Andouille</b> tongue corned beef rump pork loin shnk meatball capicola turducken venison shankle kevin
            pancetta tri-tip boudin.</p>
          <button>ANOTHER BUTTON</button>
        </div>

      </div>
    </div>

  </div>
</template>



<style>
.container1 {}

.container2 {
  width: 65%;
  margin: auto;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  color: #848484;
  line-height: 29px;
}

h1 {
  color: #585757;
  font-weight: 300;
  font-size: 35px;
  margin-bottom: 35px;
}

.content {
  display: flex;
  justify-content: space-between;
  margin: 100px 0;
}

.col1 {
  width: 54%;
}

button {
  border: none;
  padding: 15px 20px;
  border-radius: 30px;
  font-size: 10px;
  letter-spacing: 2px;
  color: white;
  font-weight: 600;
  margin-top: 26px;
}

.col1 button {
  background-color: #75bee1;
}

.col4 button {
  background-color: #95d075;

}

.col2 {
  width: 35%;

}

img {
  width: 100%;
}

.line {
  border-top: 2px solid #eef0f1;
}

.col3 {
  width: 35%;
}

.col4 {
  width: 54%;
}

/* button {
  background-color: ;
} */

</style>
