<template>
    <div class="paragraphs">

        <h1>VESTIBULUM ULLAMCORPER UT LEO QUIS</h1>
        <div class="item">
            <p>Aenean facilis lectus antem ut rutrum eros convallis et.<br> Vestibulum ullamcorper ut leo quis tristique.
                Donec in erat commodo, pharetra purus ac, consectetur lacus. Suspendisse odio sapien, egestas at ex sit
                amet, molestie sagittis est.</p>
            <p>In is purus imperdi et nisl accumsan scelerisque. Donec nec justo sed enim dapobus rhoncus. Morbi sed elit
                vitae metus ullamcorper efficitur.</p>
            <p>Fusce aliquam magna id ipsum ultricies interdum. Maecenas nibh risus.</p>
        </div>
        <button>DETAIL</button>

    </div>
</template>
<script>
export default {

}
</script>
<style scoped>
.paragraphs{
   width:70%;
   padding-left:40px ;
   box-sizing: border-box;
   line-height: 30px;
   
}
h1{
    font-weight: 400;
}
 
.paragraphs p{
    font-size: 18px;
    margin: 30px 0;
    font-weight: 300;
}
.item{
    margin: 0 0 60px 0;
}
button{
    background-color:white;
    border: 2px solid;
    border-radius: 3px;
    padding: 8px 32px;
    font-weight: 500;
    font-size:medium;
}
</style>