<template>
<div>
<ul class="list-group">
  <li class="list-group-item active bg-dark">Categories</li>
  <li class="list-group-item list-group-item-action" v-for="category in categories" :key="category.id">{{category.Catname}}</li>
  
</ul>
</div>


        
   
</template>
<script>
export default {
    name: 'sideBar',
     
     data(){
         return{
    categories:[
      {id:1, Catname: 'Fruits'},
      {id:2, Catname: 'Vegetables'},
      {id:3, Catname: 'Beverages'},
      {id:4, Catname: 'Root'},
      {id:5, Catname: 'Crop'}
      ]
         }
     }
    

    
}
</script>
<style scoped>

</style>