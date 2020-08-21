<template>
 <div id="app">
     <img src="./assets/top.jpg" style="max-width:100%;height:auto;">
    <HelloWorld msg=" WELCOME TO Thai painting works" />
    <hr>
    <img src="./assets/19027_776865.jpg" width = 50% >
    <div class="row">
      <div class="col-6">
         <CsButton @cc="sum" />
        <h1>{{total1}}</h1>
      </div>
     <img src="./assets/pj024.jpg" width = 50% >
      <div class="col-6">
        <CsButton @cc="sum1" />
         <h1>{{total2}}</h1>
      </div>
      <img src="./assets/9a5c1dd8-394d-4e36-8cb2-ffef7bc73525.jpg" width = 50% >
    
      <div class="col-6">
        <CsButton @cc="sum2" />
      <h1>{{total3}}</h1>
      </div>
    </div>
    <img src="./assets/footer.jpg" style="max-width:100%;height:auto;">
  </div>
</template>
<script>
import HelloWorld from "./components/HelloWorld.vue";
import CsButton from "./components/CSButton.vue";
export default {
  name: "App",
  components: {
    HelloWorld,
    CsButton,
    
  },
  data : function(){
    return {
    total1: 0,
    total2: 0,
    total3: 0,
   
   } 
  },
  methods: {
  sum(counterValue){
    this.total1 = counterValue
  },
  
  sum1(counterValue){
    this.total2 = counterValue
 
  
},
sum2(counterValue){
    this.total3 = counterValue
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
  color: #0b44ff;
  margin-top: 60px;
}
</style>