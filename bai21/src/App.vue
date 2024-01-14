<!-- <script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script> -->

<template>
  <div class="container">
    <div class="background">
      <div class="content">

        <div class="col1">
          <div class="border">
            <p>190 x 50</p>
          </div>
          <p>Integer rutrum ligula eu dignissim laoreet. Pellentesque venenatis nibh sed tellus faucibus bibendum. Sed
            fermentum est vitae rhoncus molestie. Cum sociis natoque penatibus et magnis dis montes.</p>
          <p>Sed dermentum est vitae rhoncus molestie. Cum sociis natoque penatibus et magnis dis montes.</p>
        </div>

        <div class="col2" v-for="x in col23">
          <h3>{{ x.title }}</h3>
          <ul>
            <li v-for="y in x.list">
              <a v-bind:href="y.link">{{ y.message }}</a>
              <address>{{ y.address }}</address>
            </li>

          </ul>
        </div>


        <div class="col4">
          <h3>{{ col4.ttitle }}</h3>
          <ul>
            <li v-for="n in col4.llist">
              <div class="col4-row">
                <div class="icon"><a v-bind:href="n.llink"><i v-bind:class="n.icon" aria-hidden="true"></i></a></div>
                <p>{{ n.para }}</p>
              </div>
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
      col23: [
        {
          title: 'Informaton Link',
          list: [
            {
              link: '#Home',
              message: 'Home'
            },
            {
              link: '#Blog',
              message: 'Blog'
            },
            {
              link: '#Pricing',
              message: 'Pricing'
            },
            {
              link: '#About',
              message: 'About'
            },
            {
              link: '#Faq',
              message: 'Faq'
            },
            {
              link: '#Contact',
              message: 'Contact'
            }
          ]
        },
        {
          title: 'Contact Details',
          list: [
            {
              link: '#info@yoursite.com',
              message: 'info@yoursite.com'
            },
            {
              link: '#www.yoursite.com',
              message: 'www.yoursite.com'
            },
            {
              link: '',
              message: '',
              address: '123 Nguyen Van B, Tp.HCM Vietnam'
            },
            {
              link: '#+61 3 8376 6284',
              message: '+61 3 8376 6284'
            },

          ]
        }
        
      ],
      col4: {
        ttitle:'Socical',
        llist: [
          {
            llink: '#22.543 Like',
            icon:'fa fa-facebook',
            para: '22.543 Like'
          },
          {
            llink: '#128 Projects',
            icon:'fa fa-github',
            para: '128 Projects'
          },
          {
            llink: '#12.860 Followers',
            icon:'fa fa-twitter',
            para: '12.860 Followers'
          },
          {
            llink: '#3312 Shots',
            icon:'fa fa-dribbble',
            para: '3312 Shots'
          },
          {
            llink: '#3331 Pins',
            icon:'fa fa-pinterest',
            para: '3331 Pins'
          },

        ]
      }
    }
  }
}
</script>

<style>
.container {
  padding: 50px 0;
}

.background {
  background-color: #1f1f1f;
  width: 85%;
  margin: auto;
  padding: 50px;

}

.content {
  color: #818181;
  display: flex;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  line-height: 30px;
  justify-content: space-between;
}

h3 {
  color: white;
  margin-top: 0;
}

.col1 {
  width: 35%;
}

.col2 {
  width: 21%;
}

.col3 {
  width: 21%;
}

.col4 {
  width: 17%;
}

.border {
  background-color: #8598cc;
  margin-bottom: 50px;
  width: 190px;
  height: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 25px;
  font-weight: 200;
}

.border p {
  color: white !important;
}



ul {
  list-style-type: none;
  padding: 0;
}

li {
  border-bottom: 1px dashed #3e3e3e;
  border-left: none;
  border-right: none;
  padding: 10px 0;
}

li:last-child {
  border-bottom: none;
}


a:link,
a:visited {
  text-decoration: none;
  color: #818181;
}

a:hover {
  color: #efe8e8;
}

.col4-row {
  display: flex;
  align-items: baseline;
}

.icon {
  padding: 0;
  width: 25px;
  height: 15px;
  border-right: 1px dashed #3e3e3e;
  display: flex;
  align-items: center;

}

.col4-row p {
  margin: 0 12px 0;
}

address {
  font-style: normal;
  padding-right: 50px;
}
</style>
