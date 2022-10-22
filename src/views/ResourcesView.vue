<template>
    <div class="resources-page">
        <h1 class="resource-title">Equine Veterinary Clinic of Tucson Resources</h1>
        <div class="row">
            <div class="resource-square">
                <img src="../assets/Resource-USDA.jpg" class="resource-img"/>
                <a href="https://www.aphis.usda.gov/aphis/ourfocus/animalhealth/animal-disease-information/equine">USDA Equine</a>
            </div>
            <div class="resource-square">
                <img src="../assets/Resource-AAEP.png" class="resource-img"/>
                <a href="https://aaep.org/horse-owners">AAEP</a>
            </div>
            <div class="resource-square">
                <img src="../assets/Resource-USEF.jpg" class="resource-img"/>
                <a href="https://www.usef.org">USEF</a>
            </div>
            <div class="resource-square">
                <img src="../assets/Resource-FEI.png" class="resource-img"/>
                <a href="https://www.usef.org">FEI</a>
            </div>
        </div>
        <div class="row">
            <div class="resource-square">
                <img src="../assets/Resource-AQHA.png" class="resource-img"/>
                <a href="https://www.aphis.usda.gov/aphis/ourfocus/animalhealth/animal-disease-information/equine">USDA Equine</a>
            </div>
            <div class="resource-square">
                <img src="../assets/Resource-Jockey.png" class="resource-img"/>
                <a href="https://aaep.org/horse-owners">AAEP</a>
            </div>
            <div class="resource-square">
                <img src="../assets/Resource-AHA.png" class="resource-img"/>
                <a href="https://www.usef.org">USEF</a>
            </div>
            <div class="resource-square">
                <img src="../assets/Resource-FEI.png" class="resource-img"/>
                <a href="https://www.usef.org">FEI</a>
            </div>
        </div>
    </div>


</template>


<style>

.resources-page{

}

.resource-title{
    text-align: center;
    margin-top: 5%;
    margin-bottom: 5%;
}

.row{
    display: flex;
    justify-content: space-evenly;
}

.resource-square{
    display: flex;
    flex-direction: column;
    padding: 20px;
    width: 400px;
    height: 300px;
    border: 2px solid white;
    align-items: center;
    box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
    margin: 20px;
    border-radius: 16px;

}

.resource-img{
    width: 200px;
    height: 200px;
}

@media (max-width: 480px){
    .resource-square{
        width: 300px;
    }
}

</style>