<!-- <template>
    <div class="about-TE">
        
        <div class="description">
            <h1 class="about-title">Welcome to Equine Veterinary Clinic of Tucson </h1>
            <p>Our mission is to provide gold standard veterinary care to the equine population of southeastern Arizona. We accomplish this through a high diagnosis rate, utilizing efficient examination techniques and the best technologies/therapies available. We strive for a simplistic client experience. Excellent client communication is vital for high quality patient care. </p>
            <button type="button" class ="about-doc-btn">Meet The Doctor</button>
        </div>
        <img src ="../assets/CS-Pic.jpg" class="about-img">
    </div>
</template>

<style scoped>

.about-TE{
    margin-top: 4%;
    background-color: #8ECAE6;
    display: flex;
    flex-direction: row;
    height: 700px;
    justify-content: space-evenly;
    
    
}



.description{
  
    display: flex;
    flex-direction: column;
    justify-content: center;

    text-align: left;
    padding-left: 200px;
    padding-right: 200px;
    color: white;

}

.about-title{
    text-align: left;
    font-weight: bold;
}
.about-doc-btn{

  width: 250px;
  border: solid 2px;
  border: white;
  background-color: White;
  border-radius: 16px;
  font-weight: bold;
  color: #8ECAE6;
  padding: 5px;
  font-size: 20px;



}
.about-doc-btn:hover {
  background-color: transparent;
  border: solid 2px;
  border-color:white ;
  color: white;
}

.about-img{
    height: 100%;
    width: 100%;




}

</style> -->

<template>
    <div class="welcome-to-box">
        <div class="description">
            <h1 class="about-title" id="title">Welcome to Equine Veterinary Clinic of Tucson </h1>
            <p>Our mission is to provide gold standard veterinary care to the equine population of southeastern Arizona. We accomplish this through a high diagnosis rate, utilizing efficient examination techniques and the best technologies/therapies available. We strive for a simplistic client experience. Excellent client communication is vital for high quality patient care. </p>
            <button type="button" class ="meet-us-btn">Meet The Team</button>
        </div>
        <img src ="../assets/CS-Pic.jpg" class="about-img">        
    </div>


</template>

<style scoped>

.welcome-to-box{
    display: flex;
    flex-direction: row;
    justify-content: center;
    background-color: #023047;
    padding-top: 50px;
    padding-bottom: 50px;
    margin-top: 5%;
 

}

img{
    width: 500px;
    height: 500px;
    margin-left: 50px;
}

.description{
    margin-top: 50px;
    display: flex;
    flex-direction: column;
    width: 500px;
    text-align: left;
    color: white;
}

#title{
    
    margin-bottom: 40px;
}

.meet-us-btn{
    margin-top: 30px;
    width: 250px;
  /* height: 4%; */
    border: white solid 2px;
    background-color: White;
    border-radius: 16px;
    font-weight: bold;
    color: #023047;
    padding: 5px;
    font-size: 20px;
    margin-bottom: 5%;
  
}

.meet-us-btn:hover {
  background-color: transparent;
  border: solid 2px;
  border-color:white ;
  color: white;
}

@media (max-width: 480px){
    .welcome-to-box{
    display: flex;
    flex-direction: column-reverse;
    justify-content: center;
    background-color: #023047;
    padding-top: 50px;
    padding-bottom: 50px;
    margin-top: 5%;
 

    }

    img{
        width: 100%;
        margin-left: 0;
    }

    .description{
        margin-top: 50px;
        display: flex;
        flex-direction: column;
        width: 100%;
        text-align: left;
        color: white;
    }
}

</style>