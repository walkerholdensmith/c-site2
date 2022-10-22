<template>
    <div class="emergency-page">
        <img src="../assets/Emergency-Page-Pic.jpg" id="emergency-img"/>
        <h1 id="emergency-title">Is your horse in need of Emergency Health Services?</h1>
        <p id="emergency-desc">Lorem ipsum dolor sit amet consectetur adipisicing elit. Exercitationem quo adipisci voluptas quaerat libero dolore, ex culpa? Quae illum saepe nostrum atque amet distinctio quis molestiae nobis nam optio. Tenetur?</p>
        <div class="list">
            <li>Fever</li>
            <li>Fever</li>
            <li>Fever</li>
            <li>Fever</li>
            <li>Fever</li>
            <li>Fever</li>

        </div>
        <p id="emergency-desc">Lorem ipsum dolor sit amet consectetur adipisicing elit. Exercitationem quo adipisci voluptas quaerat libero dolore, ex culpa? Quae illum saepe nostrum atque amet distinctio quis molestiae nobis nam optio. Tenetur?</p>
        <button type="button" class ="emergency-btn">Contact Us</button>
    </div>


</template>

<style scoped>

.emergency-page{
    display: flex;
    flex-direction: column;
    width: 100%;
    align-items: center;
    justify-content: center;

}

.list{


    margin-right: 600px;
    text-align: left;
   
}

#emergency-desc, #emergency-title{
    width: 700px;
}

#emergency-desc{
    margin-top: 20px;
}

li{
    text-align: left;
}

.emergency-img{
    /* padding: 100px; */

}

.emergency-btn{

/* transform: translate(-50%, -50%); */
width: 250px;
/* height: 4%; */
border: #8ECAE6 solid 2px;
background-color: #8ECAE6;
border-radius: 16px;
font-weight: bold;
color: white;
padding: 5px;
font-size: 20px;
margin-bottom: 5%;




}


.emergency-btn:hover {
background-color: transparent;
border: solid 2px;
border-color:#8ECAE6 ;
color: #8ECAE6;
}



</style>