<template>
    <div class="servicesV2">
        <h3 id="services-header">Some Of Our Services</h3>
        <div class="top-row">
            <div class="service-square-v2" id="Emergencies">
                <!-- <img src="../assets/CS-Emergency.png" class="service-img-v2"/> -->
                <h5 class="service-title-v2">Emergencies</h5>
                <p class="service-desc">When you need us most, we are there!</p>
                <button type="button" class="btn btn-outline-primary" id="read-more">Read More</button>
            </div>
            <div class="service-square-v2" id="wellness">
                <!-- <img src="../assets/CS-Emergency.png" class="service-img-v2"/> -->
                <h5 class="service-title-v2">Routine Wellness</h5>
                <p class="service-desc">When you need us most, we are there!</p>
                <button type="button" class="btn btn-outline-primary" id="read-more">Read More</button>
            </div>
        </div> 
        <div class="bottom-row"> 
            <div class="service-square-v2" id="sports-med">
                <!-- <img src="../assets/CS-Emergency.png" class="service-img-v2"/> -->
                <h5 class="service-title-v2">Sports Med</h5>
                <p class="service-desc">When you need us most, we are there!</p>
                <button type="button" class="btn btn-outline-primary" id="read-more">Read More</button>
            </div>
            <div class="service-square-v2" id="pre-purchase">
                <!-- <img src="../assets/CS-Emergency.png" class="service-img-v2"/> -->
                <h5 class="service-title-v2">Pre-Purchase</h5>
                <p class="service-desc">When you need us most, we are there!</p>
                <button type="button" class="btn btn-outline-primary" id="read-more">Read More</button>
            </div>
        </div>
            <!-- <div class="service-square">
                <img src="../assets/CS-Emergency.png" class="service-img"/>
                <h5 class="service-title">Emergencies</h5>
            </div> -->
            <!-- <div class="service-square">
                <img src="../assets/CS-Emergency.png" class="service-img"/>
                <h5 class="service-title">Lamness Exams</h5>
            </div>
            <div class="service-square">
                <img src="../assets/CS-Emergency.png" class="service-img"/>
                <h5 class="service-title">Gastrascope</h5>
            </div> -->
   
        <!-- <div class="bottom-row">
            <div class="service-square">
                <img src="../assets/CS-Emergency.png" class="service-img"/>
                <h5 class="service-title">Imaging</h5>
            </div>
            <div class="service-square">
                <img src="../assets/CS-Emergency.png" class="service-img"/>
                <h5 class="service-title">Euthinizations</h5>
            </div>       
        </div> -->
    </div>


</template>

<style>


/* .service-img-v2{
    height: 250px;
    width: 300px;  
    position: relative;
} */

.service-square-v2{
    background-image: url("../assets/CS-Emergency.png");
    background-size: 300px 300px;
    height: 250px;
    width: 300px;
    margin-bottom: 10px;
    border-radius: 16px;
    display: flex;
    flex-direction: column;
    text-align: center;
    align-items: center;
    justify-content: center;
    padding: 20px;
    margin: 20px;
    margin-bottom: 5%;

}

#wellness{
    background-image: url("../assets/CS-Wellness.png");
}

#sports-med{
    background-image: url("../assets/CS-Sports-Med.png");
}

#pre-purchase{
    background-image: url("../assets/CS-PP.png");
}

.service-title-v2, .service-desc{

    color: white;
    left: 50%;
    top: 50%;
}

.servicesV2{
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    background-color: #FB8500;
    margin-top: 10%;

}

#services-header{
    margin-top: 5%;
    font-size: 30px;
    font-weight: bold;
    color: white;
    align-items: center;
    text-align: center;
}

.top-row, .bottom-row{
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    margin-top: 30px;

}



.bottom-row{
    /* margin-top: -80px; */
    margin-bottom: 2%;
}

.service-square{
    display: flex;
    flex-direction: column;
    margin: 20px
}
.service-img{
    height: 250px;
    width: 300px;
}

.service-title{
    background-color: white;
    color: #023047;
    width: 300px;
    height: 50px;
    text-align: center;
    justify-content: center;
    padding-top: 10px;
    font-weight: bold;

    
}

.service-title:hover{
    background-color: #023047;
    color: white;
    width: 300px;
    height: 50px;
    text-align: center;
    justify-content: center;
    padding-top: 10px;
    font-weight: bold;

    
}

@media (max-width: 480px){
    .servicesV2{

    }

    .service-square-v2{
        background-image: url("../assets/CS-Emergency.png");
        background-size: 100px 150px;
        height: 100px;
        width: 150px;
        margin-bottom: 10px;
        border-radius: 16px;
        display: flex;
        flex-direction: column;
        text-align: center;
        align-items: center;
        justify-content: center;
        padding: 20px;
        margin: 20px;
        margin-bottom: 5%;
    }
    .service-title-v2, .service-desc{

        color: white;
        left: 50%;
        top: 50%;
        font-size: 10px;
    }

    .service-desc{
        display: none;
    }

    #read-more{
        font-size: 8px;
    }

}

</style>