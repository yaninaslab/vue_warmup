<template>
  <div id="app">
    <home-page-body></home-page-body>
  </div>
</template>

<script>
import HomePageBody from './components/HomePageBody.vue'
export default {
  name: 'App',
  components: {
    HomePageBody,
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
