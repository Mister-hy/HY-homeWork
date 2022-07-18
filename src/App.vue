<template>
  <div id="app">
    <div id="nav">
      <router-link to="/"></router-link> 
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
html,body,#app{
  width: 100%;
  height: 1000px;
  box-sizing: border-box;
  padding: 0;
  margin: 0;
  overflow: hidden;
}
ul,li{
  list-style: none;
}
p,h2,h3,h4,h5{
  padding: 0;
  margin: 0;
}
</style>
