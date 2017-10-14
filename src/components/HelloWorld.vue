<template>
  <div class="hello">
  
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your2 Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
.w{
  width: 100vw;
}
.w span{
  display: block;
  float: left;
  width: 25%;
  height: 25px;
}
.w span:nth-child(1){
  background-color: green;
}.w span:nth-child(2){
  background-color: blue;
}.w span:nth-child(3){
  background-color: yellow;
}.w span:nth-child(4){
  background-color: pink;
}
</style>
