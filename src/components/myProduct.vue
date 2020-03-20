<template>
<div>
    <div class="col-4 myprod" v-for="product in products" :key="product.myid">
            <div class="card">
               <img v-bind:src="product.ProductImage" height= "150" >
                <div class="card-body">
                    <h4 class="card-title">{{product.prodName}}</h4>
                    <div class="card-text">
                        <span>&#8358; {{product.Price}}  </span>
                        
                    </div>
                    <div class="row-justify-content-end">
                        <button class="btn btn-primary" @click="myDear()">Order Now!</button>

                    </div>
                </div>

            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'myProduct',
    methods: {
        myDear(){
           alert('I love Ummu Amina');
       }
    },
    data(){
    return{
     
      products: [
     {myid:1, prodName:'Coffee', Price:'2300', ProductImage:'/coffee.jpg', catid:1},
      {myid:2, prodName:'Pawpaw', Price:'180', ProductImage:'/pawpaw.jpg', catid:2},
      {myid:3,prodName:'GreenBeans', Price:'4450', ProductImage:'/greenBeans.jpg', catid:3},
      {myid:4, prodName:'mango', Price:'950', ProductImage:'/mango.jpg', catid:4},
      {myid:5, prodName:'banana', Price:'840', ProductImage:'/banana.jpg', catid:5},
      {myid:6,prodName:'cassava', Price:'1500', ProductImage:'/cassava.jpg', catid:5},
      {myid:7,prodName:'Apple', Price:'550', ProductImage:'/apple.jpg', catid:1},
      {myid:8,prodName:'Pineapple', Price:'150', ProductImage:'/pineapple.jpg', catid:2},
      {myid:9,prodName:'Orange', Price:'200', ProductImage:'/orange.jpg', catid:3},
      {myid:10,prodName:'mango', Price:'250', ProductImage:'/mango.jpg', catid:4},
      //{prodName:'banana', Price:'840', ProductImage:'/banana.jpg', catid:5},
      {myid:11,prodName:'kolanut', Price:'1250', ProductImage:'/kolanut.jpg', catid:1},
      {myid:12,prodName:'cocoyam', Price:'150', ProductImage:'/cocoyam.jpg', catid:2},
      {myid:13,prodName:'stawberry', Price:'200', ProductImage:'/strawberry.jpg', catid:3},
      {myid:14,prodName:'lime', Price:'250', ProductImage:'/lime.jpg', catid:4},
      {myid:17,prodName:'lemo', Price:'250', ProductImage:'/lemo.jpg', catid:4},
      {myid:18,prodName:'Guava', Price:'250', ProductImage:'/guava.jpg', catid:4},
      {myid:15,prodName:'Cucumber', Price:'100', ProductImage:'/cucumber.jpg', catid:5},
      {myid:16,prodName:'Watermelon', Price:'300', ProductImage:'/watermelon.jpg', catid:5}
     
      ]
    }
  }
   
    
}
</script>
<style scoped>
.card{
    
    margin-bottom: 40px;
}
.myprod{
    display: inline-block;
}

</style>