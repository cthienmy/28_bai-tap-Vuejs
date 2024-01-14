<template>
    <div class="navbar">
                <ul>
                    <li><a href="#ALL">ALL</a></li>
                    <li><a href="#Web App">Web App</a></li>
                    <li><a href="#UI/UX">UI/UX</a></li>
                    <li><a href="#Grapphics Design">Grapphics Design</a></li>
                    <li><a href="#Mobile App">Mobile App</a></li>
                    <li><a href="#Branding">Branding</a></li>
                    <li><a href="#Marketing">Marketing</a></li>
                </ul>
            </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
  .navbar{}

ul{
    list-style-type:none;
    display:flex;
    justify-content:center;
    margin:40px 0 30px 0;
}
 li{
padding:20px;
 }
a{
    text-decoration: none;
    color:#565656;
    font-weight:600;
}
a:hover,a:active{
color:#389b9b;
}  
</style>