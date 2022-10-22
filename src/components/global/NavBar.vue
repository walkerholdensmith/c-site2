<template>
    <div class="main-nav">
        <div class="logo-and-name">
            <!-- <img src="../assets/logo-final.png" class="logo-img"/> -->
            <!-- <p class="site-name">Equine Veterinary Clinic of Tucson</p>    -->
        </div>
  
        <ul class="nav-items">
          <!-- <img src="logo.png" class="logo-img"/> -->

          <li class="nav-item"><router-link to="/" class="item-text"><fa icon="house"/> Home</router-link> </li>
          <li class="nav-item"><router-link to="/Services" class="item-text"><fa icon="hospital"/> Services</router-link></li>
          <li class="nav-item"><router-link to="/About" class="item-text"><fa icon="address-card"/> About</router-link></li>
          <li class="nav-item"><router-link to="/Contact" class="item-text"><fa icon="address-book"/> Contact</router-link></li>
          <li class="nav-item"><a href="#" class="item-text"><fa icon="circle-info"/> Resources</a></li>
          <li class="nav-item"><router-link to="/Emergency" class="item-text"><fa icon="truck-medical"/> Emergency</router-link></li>
          <li>        
            <div class="call-us">
            <p class="call-item">Call Us</p>
            <p class="call-item"><fa icon="phone"/>  (520)247-4003</p>
            </div>
          </li>
        </ul>


        
    </div>

</template>

<style scoped>
.main-nav{
    display: flex;
  
    height: 80px;
    z-index: 99;
    background-color: #FB8500;
}

.logo-img{
    height: 200px;
    width: 250px;
    z-index: 101;
    /* position: fixed; */
    top: 0;
    /* background-color: #FB8500; */
    /* padding-left: 10px; */
    margin-left: 200px;
    margin-top: -60px;
    /* padding-top:-20px; */
}

.nav-items{
    background-color: #FB8500;
    width: 100%;
    display: flex;
    height: 80px;
    list-style: none;
    justify-content: center;
    text-align: center;

    position: fixed;
    top: 0;
    z-index: 100;
    
}

.nav-item{
    margin-left: 20px;
    margin-right: 20px;
    padding-top: 25px;
    

}


.item-text{
    color: white;
    text-decoration-line: none;
    font-weight: bold;
    font-size: 18px;
}

.item-text:hover{
    color: rgba(142, 202, 230, .65);
}

.site-name{
    color: white;
    padding-top: 25px;
    padding-left: 10px;
    font-weight: bold;
    font-size: 18px;

}


.logo-and-name{
    z-index: 101;
    position: fixed;
    display: flex;
}

.call-us{
    /* position: fixed; */
    top: 0;
    /* left: 75%; */
    z-index: 101;
    display: flex;
    flex-direction: column;
}

.call-item{
    padding-top: 10px;
    margin: 0;
    font-weight: bold;
    color: white;
}


@media(max-width: 992px){
    .main-nav{
        display: flex;
        flex-direction: row;
    }
}
</style>