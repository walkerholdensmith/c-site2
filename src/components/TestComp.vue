<template>
<nav class="navbar navbar-expand-lg" style="background-color:#FB8500">
  <div class="container-fluid" >
    
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNavDropdown" >
      <ul class="navbar-nav" >
        <li class="nav-item">
          <router-link to="/" class="nav-link" style="color: white;"><fa icon="house"/> Home</router-link>
        </li>

        <li class="nav-item">
          <router-link to="/About" class="nav-link" style="color: white;"><fa icon="address-card"/> About</router-link>
        </li>
        <li class="nav-item dropdown">
          <router-link to="/Services" class="nav-link dropdown-toggle" role="button" data-bs-toggle="dropdown" aria-expanded="false" style="color: white;"> Services</router-link>
          <ul class="dropdown-menu">
            <li><router-link to="/Services" class="dropdown-item" role="button" data-bs-toggle="dropdown" aria-expanded="false" style="color: black;"> Services</router-link></li>
            <li><a class="dropdown-item" href="#">Another action</a></li>
            <li><a class="dropdown-item" href="#">Something else here</a></li>
          </ul>
        </li>
        <!-- <fa icon="circle-info" /> -->
        <li class="nav-item"><router-link to="/Contact" class="nav-link" style="color: white;"><fa icon="address-book"/> Contact</router-link></li>
        <li class="nav-item"><router-link to="/resources" class="nav-link" style="color: white;"><fa icon="circle-info"/> Resources</router-link></li>
        <li class="nav-item"><router-link to="/Emergency" class="nav-link" style="color: white;"><fa icon="truck-medical"/> Emergency</router-link></li>
        <!-- <li class="nav-item"><fa icon="phone"/>Call Us </li> -->
      </ul>
      <!-- <img src="../assets/logo-final.png" class="logo-img"/> -->
    </div>
  </div>
</nav>

</template>


<style>
.navbar {
    background-color: lightgreen;
    height: 100px;
    
}

.nav-item{
  font-weight: bold;
  padding-left: 20px;
 
}

.nav-link{
  color: white;
}

.logo-img{
    height: 150px;
    width: 150px;
    z-index: 101;
    margin-top: -50px;
    /* position: fixed; */
    /* top: 0; */
    /* background-color: #FB8500; */
    /* padding-left: 10px; */
    margin-left: 500px;
    /* margin-top: -60px; */
    /* padding-top:-20px; */
}

</style>