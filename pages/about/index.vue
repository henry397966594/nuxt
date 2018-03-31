<template>
  <div class="main">
    <section id="about-page">
      <h1>Hi, that's us </h1>
      <p>who will be the first</p>
     </section>
  </div>
</template>

<script>
    export default {
  transition:'test'
}
</script>   
<style>
.main #about-page{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    
}
.main #about-page h1{
    position: relative;
    filter: 0;
    transition: filter 1.5s ease;
     animation: move 2s cubic-bezier(0.23, 1, 0.320, 1)
}
#about-page p{
    font-size: 20px;
    font-weight: 700;
    position: relative;
    animation: mymove 2s ease-in;
}
@keyframes mymove{
from {left:300px;}
to {left:0px;}

}
@keyframes move {
    from{right:300px;}
    to{right:0px;}
    from{color:rgb(145, 255, 0);}
    to{
        color:black;
    }
}
</style>

