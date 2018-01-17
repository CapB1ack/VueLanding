<template>
  <div id="app">
    <Landing/>
  </div>
</template>

<script>
import Landing from './components/Landing'

export default {
  name: 'app',
  components: {
    Landing
  }
}
</script>

<style>
  @import url('../node_modules/roboto-fontface/css/roboto/roboto-fontface.css');
  body, html {
    margin: 0;
    padding: 0;
  }
#app {
  font-family: 'Roboto', sans-serif;
  font-weight: 300;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
