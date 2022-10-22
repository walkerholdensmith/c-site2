<template>
    <div class="request-appointment-bar">
        <h3 class="request-title">Routine Checkup?</h3>
        <button type="button" class ="emergency-btn">Contact Us</button>
    </div>

</template>

<style scoped>

.request-appointment-bar{
 /* padding-top: 25%; */
 background-color: #FB8500;
 display: flex;
 flex-direction: column;
 align-items: center;
 justify-content: space-evenly;
 /* height: 200px; */

}

.request-title{
    padding-top: 5%;
    color: white;
    font-weight: bold;
    font-size: 40px;
    margin-bottom: 20px;
}

.emergency-btn{

  /* transform: translate(-50%, -50%); */
  width: 250px;
  /* height: 4%; */
  border: white solid 2px;
  background-color: White;
  border-radius: 16px;
  font-weight: bold;
  color: #8ECAE6;
  padding: 5px;
  font-size: 20px;
  margin-bottom: 5%;
  



}


.emergency-btn:hover {
  background-color: transparent;
  border: solid 2px;
  border-color:white ;
  color: white;
}

@media (max-width: 480px){
  .request-appointment-bar{
 /* padding-top: 25%; */
 background-color: #FB8500;
 display: flex;
 flex-direction: column;
 align-items: center;
 justify-content: space-evenly;
 /* height: 200px; */

}

.request-title{
    padding-top: 5%;
    color: white;
    font-weight: bold;
    font-size: 20px;
    margin-bottom: 20px;
}

.emergency-btn{

  /* transform: translate(-50%, -50%); */
  width: 150px;
  /* height: 4%; */
  border: white solid 2px;
  background-color: White;
  border-radius: 16px;
  font-weight: bold;
  color: #8ECAE6;
  padding: 5px;
  font-size: 15px;
  margin-bottom: 5%;
  



}


.emergency-btn:hover {
  background-color: transparent;
  border: solid 2px;
  border-color:white ;
  color: white;
}

}

</style>