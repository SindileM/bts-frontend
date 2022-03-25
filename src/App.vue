<template>
<div>
   <Navbar/>
  <img alt="Vue logo" src="https://i.postimg.cc/htgfL1Rj/bts-festa-2020-group-concept-photo-hybe-big-hit-music.jpg">
  <Home msg="Welcome to BTS BLOG"/>
</div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Home from './components/Home.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Home,
    
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
