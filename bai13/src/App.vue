<script setup>
import head3 from './components/h3.vue'
import liA from './components/item.vue'
</script>

<template>
  <div class="container">
    <div class="content">

      <div class="col1">
        <head3 title="Air" />
        <div class="item1">Facilis ipsum reprehenderit nemo molestias. Aut cum mollitia reprehenderit. Eos cumque dicta
          adipisci architecto culpa amet.</div>
      </div>

      <div class="col2">
        <head3 title="Link" />
        <div class="item1">
          <ul>
            <liA link="#Home" message="Home" />
            <liA link="#Portfolio" message="Portfolio" />
            <liA link="#Blog" message="Blog" />
            <liA link="#About" message="About" />
          </ul>
        </div>
      </div>

      <div class="col3">
        <head3 title="Categories" />
        <div class="item1">
          <ul>
            <liA link="#Landing Page" message="Landing Page" />
            <liA link="#Real Estate" message="Real Estate" />
            <liA link="#Personal" message="Personal" />
            <liA link="#Business" message="Business" />
            <liA link="#e-Commerce" message="e-Commerce" />
          </ul>
        </div>
      </div>

      <div class="col4">
        <head3 title="Contact Infomation" />
        <address class="item1">
          <p>198 West 21th Street,<br> Suite 721 New York NY 10016</p>
          <ul>
            <liA link="#+ 1235 2355 98" message="+ 1235 2355 98" />
            <liA link="#info@yoursite.com" message="info@yoursite.com" />
          </ul>


        </address>
      </div>

    </div>
  </div>
</template>

<style>
.container {
  padding-top: 100px;
}

.content {
  width: 80%;
  margin: auto;
  display: flex;
  color: #bababa;
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  line-height: 30px;
  font-size: 19px;
  color: #737373;
  letter-spacing: 1px;

}

.col2,
.col3 {
  flex-basis: 20%;
}

.col4 {
  flex-basis: 26%;
}

.col1 {
  flex-basis: 34%;
  padding-right: 120px;
}



ul {
  list-style-type: none;
  padding: 0;
}


address {
  font-style: normal;
}
</style>
