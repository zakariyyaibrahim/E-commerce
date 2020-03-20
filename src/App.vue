<template>
  <div id="app">
  <MyHeader/>
  <Carrosel/>
  <div class="container">
    <div class="row">
      <div class="col-md-3">
         <myCategory/>

      </div>
      <div class="col-md-8">
        <myProduct/>

      </div>
    </div>
  </div>
 
  
  <myFooter/> 
  
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import MyHeader from './components/MyHeader.vue'
import MyFooter from './components/MyFooter.vue'
import myCategory from './components/myCategory.vue'
import myProduct from './components/myProduct.vue'
import Carrosel from './components/Carrosel.vue'

export default {
  name: 'App',
  components: {
    //HelloWorld,
    MyHeader,
    MyFooter,
    myCategory,
    myProduct,
    Carrosel
  }
}
</script>

<style>
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
#app{
  background-color:grey;
}
</style>
