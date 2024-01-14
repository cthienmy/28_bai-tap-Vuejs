<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <div class="container">
        <div class="content">

            <h3>Get in touch with us by filling contact form below</h3>
            
            <div class="form">
                
                <form>
                    <div class="row1">
                        <input class="name" type="text" placeholder="* Enter your full name">
                        <input class="email" type="email" placeholder="* Enter your email address">
                    </div>
                    <input type="text" placeholder="Enter your subject">
                    <textarea class="message" type="text" placeholder="* Your message here..."></textarea>
                </form>
               
            </div>

            <div class="foot">
                <button>Send message</button>
                <p>*Please fill all required form field, thanks!</p>
            </div>
        </div>
    </div>
</template>

<style>
.container{
    padding: 50px 0;
}

.content{
    width: 52%;
    margin: auto;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

h3{
    font-weight: 600;
    color:rgb(58, 58, 58) ;
}

.form{}

.row1{
    display: flex;
    justify-content: space-between;
}
input, textarea{
    display: block;
    margin-bottom: 10px;
    width: 100%;
    box-sizing: border-box;
    border: 2px solid #e5e3e3;
    border-radius: 2px;
    padding: 10px 20px;
    outline: none;
   
}
input:focus, textarea:focus{
    border: 2px solid #b2b0b0;
}
.name{
    width: 48%;
}
.email{
    width: 48%;
}

textarea{
    height: 250px;
   
}

.foot{
    display: flex;
    justify-content: space-between;
}

button{
    background-color: #7dcefd;
    border:2px solid #6bbbe9;
    color:white;
    border-radius: 3px;
    height: 40px;
    width: 120px;

}

.foot p{
    color: #757474;
}

</style>
