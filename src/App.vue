<template>
  <div id="app">
    <!-- <img src="./assets/logo.png"> -->
    <search/>
    <maincon/>
    <foot/>
  </div>
</template>

<script>
import search from './components/search'
import maincon from './components/maincon'
import foot from './components/foot'
export default {
  name: 'app',
  components: {
    search,
    maincon,
    foot
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
