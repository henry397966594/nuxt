<template>
<div class="main">
    <h2>Go to Hell</h2>
    
    <li><nuxt-link :to="{name:'post-id',params:{id:123}}" class="nuxt">one</nuxt-link></li>
   
    <li><nuxt-link to="/post/456" class="nuxt">two</nuxt-link></li>
    <li><nuxt-link to="/post/567" class="nuxt">three</nuxt-link></li>
    
    
</div>
</template>
<script>

</script>
<style scoped>
.main{
    display: flex;
    align-items: center;
    justify-content: center;  
    flex-direction: column 
}
li{
    list-style: none;
    
}
.nuxt{
    list-style: none;
    font-size: 20px;
    margin-top: 1.5rem;
    text-decoration: none;
    
}
.nuxt:hover{
    color: rgb(0, 255, 128);
    font-size: 25px;
    transition: all 1s ease-in
}
.main h2{
    position: relative;
    animation: mymove 2s cubic-bezier(0.64, 0.17, 0.85,-0.49) .5s;
}
@keyframes mymove
{
from {left:200px;}
to {left:0px;}
}

</style>