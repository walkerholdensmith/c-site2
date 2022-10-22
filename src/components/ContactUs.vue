<template>
    
    <div class="contact-us-container">
        
        <form class="contact-info">
            <h2 id="contact-title">Contact Us</h2>
            <input type="text" class="form-item" id="name-input" name="name" placeholder="Enter Name (Required)"/>
            <input type="text" class="form-item" id="name-input" name="horse-name" placeholder="Enter Horse Name (Required)"/>
            <input type="text" class="form-item" id="email-input" placeholder="Enter Email (Required)"/>
            <input type="text" class="form-item" id="phone-input" placeholder="Enter Phone (Required)"/>
            <textarea type="text" class="form-item" id="notes-input" placeholder="Notes for Doctor"></textarea>
            <input type="submit" value="Submit" id="submit-btn"/>
        </form>
        <div class="desc-v-stack">
            <h2 id="info-title">What we can do for you</h2>
            <p id="desc-second-line">Our team of experts is here to make your experience high-quality so that you receive the best service in Tucson.</p>
            <div class="desc-top-row">
                <div class="item">
                    <h6 class="section-title"><b>Quality Services</b></h6>
                    <p>Our staff is trained in the most up-to-date techniques and procedures to care for your horse.</p>
                </div>
                <div class="item">
                    <h6 class="section-title"><b>Modern Equipment</b></h6>
                    <p>We've invested in the newest equipment to deliver the best results. </p>
                </div>

            </div>
            <div class="desc-bottom-row">
                <div class="item">
                    <h6 class="section-title"><b>Friendly communication</b></h6>
                    <p>We pride ourselves on providing efficient conversation to all clients, whether you have been with us for years or are brand new. </p>
                </div>
                <div class="item">
                    <h6 class="section-title"><b>Individual Approach</b></h6>
                    <p>No two horses are alike. We focus on caring for the needs of each individual animal.</p>
                </div>   
            </div>
        </div> 

        
    </div>


</template>

<style scoped>
.contact-us-container{
    display: flex;
    flex-direction: row;
    justify-content: center;
    margin-top: 5%;
}
.contact-info{
    display: flex;
    flex-direction: column;
    width: 600px;
    margin-right: 44px;

}

.form-item{
    margin-top: 2%;
    height: 40px;
    box-sizing: border-box;
    border: 2px solid #ccc;
    -webkit-transition: 0.5s;
    transition: 0.5s;
    outline: none;
    border-radius: 5px;
}

.form-item:focus{
    border: solid  2px #FB8500;
}
#notes-input{
    height: 200px;
}

#contact-title, #info-title{
    text-align: left;
    color: #8ECAE6;
    font-weight: bold;
}

#submit-btn{
    margin-top: 2%;
    width: 20%;
    height: 40px;
    border-radius: 16px;
    font-weight: bold;
    border: solid 2px #8ECAE6;
    color: #8ECAE6;
    background-color: white;
}


#submit-btn:hover{
    border: solid 2px #8ECAE6;
    color: white;
    background-color: #8ECAE6;
}



.desc-v-stack{
    display: flex;
    flex-direction: column;
    width: 500px;
    text-align: left;
}

#info-title{
    margin-bottom: 40px;
    margin-left: 10px;
}

#desc-second-line{
    margin-left: 10px;
}

.desc-top-row,.desc-bottom-row{
    display: flex
}

.item{
    display: flex;
    flex-direction: column;
    width: 50%;
    margin: 10px;
}

@media (max-width: 480px){
    .contact-us-container{
        display: flex;
        flex-direction: column-reverse;
        width: 100%;
        padding: 10px;
    }
    .contact-info{
        display: flex;
        flex-direction: column;
        width: 100%;
        margin-right: 44px;

    }
    .desc-v-stack{
        display: flex;
        flex-direction: column;
        width: 100%;
        text-align: left;
    }
}

</style>

