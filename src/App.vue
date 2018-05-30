<template>
  <div id="app">
    <div class="header">
      <div class="logo">
        <img src="./assets/logo.png" alt="">
      </div>
      <div class="nav">
          <div>WORKS</div>
          <div>News</div>
          <div>Thinking</div>
          <div>About us</div>
      </div>
    </div>
    <div class="banner">
      <img src="./assets/banner.jpg">
    </div>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0;
  padding: 0;
}
.header, .banner{
  width: 87.6%;
  margin: 0 auto;
  margin-top: 36px;
}
.header{
  display: flex;
  justify-content:space-between;
}
img{
  width: 100%;
  height: 100%;
}
.logo{
width: 20%;
}
.nav{
  display: flex;
}
.nav div{
  padding: 20px 10px 0px 10px;
}
.nav div::after{
  width: 1px;
  background: #000000;
}
</style>
