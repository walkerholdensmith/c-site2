<template>
  <div class="about-page">
    <div class="about-nav">    
        <ul class="about-nav-list">
          <li class = "list-item" id="right" @click="this.whoWeAre=true" style="cursor:pointer">Who We Are</li>
          <li class = "list-item"><div class="vl"></div></li>
          <li class = "list-item"  @click="this.whoWeAre=false" style="cursor:pointer">Meet the Team</li>
        </ul>
    </div>
  
  </div>

  <div class="who-we-are" v-if="this.whoWeAre ===true">
    <div class="who-we-are-text">
      <h2>Who We Are</h2>
      <p> The Equine Veterinary Clinic of Tucson is a mobile veterinary clinic designed to provide leading services to patients around southeastern Arizona. As a native of Tucson, Dr. Chauncey Smith established the clinic for the community and region that stoked his love for the animal and industry. Equipped to render the highest-quality medicine available, we look forward to caring for your equine loved-ones. .</p>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestiae a repellat aspernatur similique, perferendis eligendi placeat, laborum saepe odit magni doloremque vero dolorum totam deleniti ab ullam tempore voluptatum fugit. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Reiciendis totam et a veritatis. Qui dolores iusto quos totam eaque ipsa, maxime eveniet necessitatibus atque expedita officiis laboriosam doloremque veniam sunt?Lorem ipsum dolor sit amet consectetur adipisicing elit. Illo quod asperiores quis veniam maiores autem cum optio nihil sunt, provident libero adipisci sapiente eaque debitis voluptatem repudiandae beatae reprehenderit natus.</p>
    </div>
    

    <img src="../assets/about.png" id="about-img"/>
  </div>
  <div class="meet-the-team" v-if="this.whoWeAre ===false">

    <div class="meet-container">
      <h2 class="meet-desc" id="meet-title">Head Vet</h2>
      <img src="../assets/CS-Pic.jpg" id="meet-img"/>
      
      <h3 class="meet-desc">Chauncey B. Smith DVM</h3>
      <p class="meet-desc" id="para">Dr. Chauncey B. Smith is a General Practitioner that specializes in Equine Sports Medicine and Management care. Dr. Smith is a native of Tucson, Arizona. He received his undergraduate education at the University of Arizona. He was an active equestrian in the region, earning national accolades as a competitor. Dr. Smith received his veterinary degree from The Ohio State University. He worked as an Associate Veterinary at the Cleveland Equine Clinic, where he received mentorship from leaders in the Equine Sports Medicine field. Dr. Smith is committed to the equine athlete and providing unmatched care to patients around southeastern Arizona. </p>
    </div>
    <div class="meet-container">
      <h2 class="meet-desc" id="meet-title">Manager</h2>
      <img src="../assets/meet-hannah.png" id="meet-img"/>
      
      <h3 class="meet-desc">Hannah Smith</h3>
      <p class="meet-desc" id="para">Mrs. Hannah Smith grew up as an equestrian in Columbus, Ohio. She graduated from The Ohio State University. As manager, Hannah strives for an excellent client experience. Having seen the industry from the perspectives of the equestrian and the veterinarian, Hannah excels in bridging the gap of communication for efficient patient care. </p>
    </div>   
    <div class="meet-container">
      <h2 class="meet-desc" id="meet-title">Technician </h2>
      <img src="../assets/meet-telluride.png" id="meet-img"/>
      
      <h3 class="meet-desc">Telluride Smith</h3>
      <p class="meet-desc" id="para"> Mr. Telluride Smith is eager to provide unmatched care and compassion to the clients of The Equine Veterinary Clinic of Tucson.
</p>
    </div>   

  </div>

</template>

<style scoped>

#meet-title{
  font-weight: bold;
}

.about-nav{
  background-color: #023047;
  align-items: center;
}

.about-nav-list{
  display: flex;
  justify-content: space-evenly;
  padding-top: 20px;
}

.vl {
  border-left: 3px solid white;
  height: 20px;
}

.list-item{
  list-style: none;
  color: white;
  font-weight: bold;
  padding-bottom: 10px;
}


.who-we-are{
  display: flex;
  align-items: center;
  margin-top: 10%;
}

.who-we-are-text{
  text-align: left;
  margin-left: 50px;
}

#about-img{
  height: 500px;
  margin-right: 50px;
}

.meet-the-team{
  display: flex;
  justify-content: space-evenly;
  margin-top: 5%;
}

.meet-container{
  width: 400px;

}

#para{
  text-align: left;
}

.meet-desc{
  margin: 0;
}

#meet-img{
  height: 450px;
  width: 400px;
  margin-bottom: 20px;
}

@media (max-width: 480px){
  .who-we-are{
    flex-direction: column-reverse;
  }

  #about-img{
    width: 100%;
    margin: 0;
  }

  .who-we-are-text{
    margin-top: 20px;
    margin-left: 0;
    padding: 5px;
  }

  .meet-the-team{
    flex-direction: column;
  }

  .meet-container{
    margin-top: 20px;
    margin-bottom: 20px;
  }
}


</style>


<script>
export default{
  name: 'about-page',
  data(){
    return{
      whoWeAre: false,
    }
     
  }

}

</script>