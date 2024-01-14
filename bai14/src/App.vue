<script setup>


</script>

<template>
  <div class="container">
    <div class="content">

      <div class="head">
        <h1>Powerful template features</h1>
        <p>Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenatos. Nulia nunc dui,
          tristique in sempet vel, congue sed ligula. Nam dolor ligula, faucibus id sodales in, auctor fringill torquent
          per conubia nostra.</p>
      </div>

      <div class="list">


        <div class="col" v-for="y in col">
          <ul>
            <li v-for="x in y.list">
              <i class="fa fa-check" aria-hidden="true"></i>
              <a v-bind:href="x.link">{{ x.message }}</a>
            </li>
          </ul>
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
          list: [
            { link: '#Custom Shortcodes', message: 'Custom Shortcodes' },
            { link: '#Visual Page Buider', message: 'Visual Page Buider' },
            { link: '#Unlimited Shortcodes', message: 'Unlimited Shortcodes' },
            { link: '#Responsive Theme', message: 'Responsive Theme' },
            { link: '#Tons of Layouts', message: 'Tons of Layouts' }

          ]
        },
        {
          list: [
            { link: '#Custom Shortcodes', message: 'Custom Shortcodes' },
            { link: '#Visual Page Buider', message: 'Visual Page Buider' },
            { link: '#Unlimited Shortcodes', message: 'Unlimited Shortcodes' },
            { link: '#Responsive Theme', message: 'Responsive Theme' },
            { link: '#Tons of Layouts', message: 'Tons of Layouts' }

          ]
        },
        {
          list: [
            { link: '#Custom Shortcodes', message: 'Custom Shortcodes' },
            { link: '#Visual Page Buider', message: 'Visual Page Buider' },
            { link: '#Unlimited Shortcodes', message: 'Unlimited Shortcodes' },
            { link: '#Responsive Theme', message: 'Responsive Theme' },
            { link: '#Tons of Layouts', message: 'Tons of Layouts' }

          ]
        }

      ]

    }
  }
}
</script>

<style>
.container {
  padding-top: 100px;
}

.content {
  width: 45%;
  margin: auto;
  font-family: Arial, Helvetica, sans-serif;
  color: #8d8c8c;
  line-height: 26px;
  font-size: 17px;

}

.head {}

h1 {
  color: rgb(34, 33, 33);
  margin: 30px 0;
}

.list {
  display: flex;
  justify-content: space-between;
}

.col {}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  margin-bottom: 6px;

}

i {
  color: #c2d82e;
  margin-right: 5px;
}

a:link,
a:visited {
  text-decoration: none;
  color: #a6a5a5;
  font-size: 15px;
}

a:hover,
a:active {
  color: #515050;
}
</style>
