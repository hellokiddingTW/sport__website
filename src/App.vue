<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style lang="scss">
@import './assets/all';

body{
  background-color: #fff;
}

#app{
  background-color: #000
}
ul, ol{
  list-style: none;
  padding:0;
  margin: 0;
}

@media (min-width:576px){
  body{
    width: 576px;
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
    border:2px solid #cecece;
    margin: 1rem;
  }
}

</style>
