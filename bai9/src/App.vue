<script setup>
import liA from './components/list.vue'

</script>

<template>
  <div class="container">
    <div class="content">

      <div class="head">
        <h3>Popular Tags</h3>
      </div>

      <div class="list">
        <ul>
          <liA link="#course" message="course" />
          <liA link="#web design" message="web design" />
          <liA link="#development" message="development" />
          <liA link="#language" message="language" />
          <liA link="#teacher" message="teacher" />
          <liA link="#speaking" message="speaking" />
          <liA link="#material" message="material" />
          <liA link="#css3" message="css3" />
          <liA link="#html" message="html" />
          <liA link="#learning" message="learning" />
        </ul>
      </div>
    </div>
  </div>
</template>

<style>
.container {
  display: flex;
  justify-content: center;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  margin-top: 100px;
}

.content {
  width: 20%;
}

.head {
  padding: 20px 5px;

}

h3 {
  margin: 0;
}

.list {}

ul {
  list-style-type: none;
  display: flex;
  flex-wrap: wrap;
  padding: 0;
  font-size: 12px;
  font-weight: 500;
}
</style>
