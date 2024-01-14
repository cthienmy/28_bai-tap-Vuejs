<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
   <div class="container">
        <div class="content">

          <div class="head">
            <h1>Wireframe Connects the Underlying<br>Conceptual Structure</h1>
          </div>

          <div class="foot">
            
            <div class="col1">
                <div class="letter">
                    <div class="letter-content">
                        <h2>Wireframe Connects the Underlying Conceptual Structure</h2>
                        <p>Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts far from the countries Vokalia and Consonantia, there live the blind texts.</p>
                        <p>Louie Jie Mahusay</p>
                        <a href="#">CEO, Founder</a>
                    </div>
                </div>
            </div>

            <div class="col2">

                <div class="col2-content">
                    <p>Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts far from the countries Vokalia and Consonantia, there live the blind texts.</p>
                    <p>Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts far from the countries Vokalia and Consonantia, there live the blind texts.</p>
                    <p>Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts far from the countries Vokalia and Consonantia, there live the blind texts. Far away, behind the word mountains, far from the countries Voklia and Consonantia, there live the blind texts far from the countries Vokalia and Consonantia there live the blind texts.</p>
                </div>
               
            </div>
          </div>

        </div>
    </div>

</template>

<style>
.container{
    padding: 50px 0;
}

.content{
    width:80%;
    margin:auto;
    font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 30px;
    word-spacing: 5px;
    font-size: 17px;
}

.head{
    text-align: center;
    margin-bottom: 100px;
}
h1, h2{
    font-weight: 400;
    color: #383838;
    
}

h1{
    line-height: 60px;
    font-size: 40px;
}
h2{
    line-height: 40px;
}

.foot{
    display: flex;
}

.col1{
    width: 36%;
}

.letter{
    box-shadow:1px 1px 18px   rgb(218, 216, 216);
    padding: 30px 50px 50px;
    color: #969696;
}
a{
    text-decoration: none;
    font-size: 14px;
    color:#849bbb;
    font-weight: 500;
}
.letter-content p:nth-child(3){
    margin-bottom: 0;
   font-weight: 500;
   color: #383838;
}


.col2{
    width:64%;
    padding-left: 80px;;
}

.col2-content{
    color:#616161;
}

.col2-content p:nth-child(1){
    margin-top: 0;
}

.col2-content p:nth-child(2){
    margin-top: 0;
    color: #2a2a2a;
    font-weight: 500;
    margin: 25px 0;
}
</style>
