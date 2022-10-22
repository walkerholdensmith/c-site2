<template>
    <div class="link-row">
        <div class="square">

            <h1 class="icon"><fa icon="phone"/></h1>
            <h5 class="square-title">Contact Us</h5>
            <p class="square-desc">Call or send us an email today! Our staff will respond as soon as possible.</p>

        </div>    
        <div class="square">
            <h1 class="icon"><fa icon="file-pdf"/></h1>
            <h5 class="square-title">Online Forms</h5>
            <p class="square-desc">Our patient forms are available online and can be completed in the privacy of your own home or office.</p>

        </div>    
        <div class="square">
            <h1 class="icon"><fa icon="clipboard-list"/></h1>
            <h5 class="square-title">Services</h5>
            <p class="square-desc">We strive to provide complete care for our patients. Learn more about all the services we provide.</p>
        </div>    
    </div>

</template>

<style scoped>
.link-row{
    display: flex;
    flex-direction: row;
    margin-top: 5%;
    justify-content: center;
    justify-content: space-evenly;
    
}

.square{
    width: 350px;
    height: 250px;
    padding: 50px;
    display: flex;
    flex-direction: column;
    background-color: rgba(142, 202, 230, .15);
    align-items: center;
    justify-content: center;
    transition: all .2s ease-in-out; 
}

.square-title{
    font-weight: bold;
}

.square:hover{
    transform: scale(1.1); 
    background-color:#8ECAE6 ;
}

@media (max-width: 480px){
    .square{
        width: 75px;
        height: 75px;
        /* padding: 5px; */

        display: flex;
        flex-direction: column;
        background-color: rgba(142, 202, 230, .15);
        align-items: center;
        justify-content: center;
        transition: all .2s ease-in-out; 
    }

    .icon{
        margin-top: 5px;
    }

    .square-title{
        font-size: 10px;
    }

    .square-desc{
        font-size: 0;
    }
}
</style>