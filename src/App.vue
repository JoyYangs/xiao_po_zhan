<template>
  <div id="app">
    <router-view/>
    <home></home>
  </div>
</template>

<script>
import Home from './views/Home'

export default {
  name: "App",
  components: {
    Home
  }
}
</script>

<style>
body {
  margin: 0px;
  padding: 0px;
}
a {
  text-decoration: none;
  color: white;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
}
</style>
