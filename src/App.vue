<template>
  <div id="app">
    <img alt="Vue logo" src="image/mar.jpg" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <h1>{{total}}</h1>
    <div class="row">
      

      <div class="col-3"><counter lable="Start" @cc="sum" /></div>
      <div class="col-3"><counter lable="Attack" @cc="sum" /></div>
      <div class="col-3"><counter lable="Speacial Attack" @cc="sum" /></div>

    </div>




</div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Counter from "./components/Counter.vue";
export default {
  name: "App",
  components: {
    HelloWorld,
    Counter,
  },
  data: function(){
    return{
      total: 0,
      name:'',
      code:'',
      gpa:'0.0',
  }
  },
methods : {
  // 3. 
  sum(counterValue){
    this.total += counterValue
   
  },

},

};
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
body{
background-image: url(https://f.ptcdn.info/379/058/000/pb598x6k62jRE54NdyM-o.png);
background-size: 150%;
}
</style>

