<template>
    <div class="jumbotron bg-dark"> <h1>My Online food Store</h1> 

    <marquee behavior="scroll" direction="left" >Zakariyya Online food order Company Nigerian Limited <br>
    Call Us : 08053344365, 08130600623, 08154819245 <br> Or email us: zakariyyum2@gmail.com 
    </marquee><br>
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
  <a class="navbar-brand" href="#">Navbar</a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarNav">
    <ul class="navbar-nav">
      <li class="nav-item active">
        <a class="nav-link" href="#">Food Category <span class="sr-only">(current)</span></a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Products</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Pricing</a>
      </li>
      <li class="nav-item">
        <a class="nav-link disabled" href="#">Disabled</a>
      </li>
    </ul>
  </div>
</nav>
    </div>
</template>
<script>
export default {
    name: 'MyHeader'
    
}
</script>
<style scoped>
h1, marquee{
    
    color: honeydew;
}



</style>