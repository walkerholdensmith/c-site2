<template>

<div id="container">
  <img id="image" src="../assets/welcome-v4-dark.png" />
  <div class="text-box">
    <h1 class="welcome-title">Welcome To The Equine Veterinary Clinic of Tucson</h1>
    <div class="typewriter">
      <h1>"Providing Lifelong care to the ultimate athlete"</h1>
    </div>
 
    <button class="button">Request Appointment</button>

  </div>

</div>
</template>
    
<script>


</script>

<style scoped>
#container {
  text-align: center;
  color: white;
  /* width: 100%; */
  align-items: center;
  margin: 0px, 0px, 0px, 0px;
}
#image {
  /* height: 400px; */
  width: 100%;
  position: relative;
}
.text-box {
  z-index: 100;
  position: absolute;
  color: white;
  /* color: #023047; */
  font-size: 24px;
  font-weight: bold;
  top: 50%;
  text-align: center;
  align-items: center;
  width: 100%;
  display: flex;
  flex-direction: column;
}

.welcome-title{
  font-size: 70px;
  font-weight: bold;
  color: white;
  width: 900px;
}

.typewriter h1 {
  overflow: hidden; /* Ensures the content is not revealed until the animation */
  border-right: .15em solid orange; /* The typwriter cursor */
  white-space: nowrap; /* Keeps the content on a single line */
  margin: 0 auto; /* Gives that scrolling effect as the typing happens */
  letter-spacing: .1em; /* Adjust as needed */
  animation: 
    typing 2s forwards,
    blink-caret .75s step-end infinite;
}

/* The typing effect */
@keyframes typing {
  from { width: 0 }
  to { width: 100% }
}

/* The typewriter cursor effect */
@keyframes blink-caret {
  from, to { border-color: transparent }
  50% { border-color: orange; }
}

.button {
  margin-top: 2%;
  background-color: white;
  border: solid white 2px;
  color: #023047;
  font-weight: bold;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  /* display: inline-block; */
  /* margin: 4px 2px; */
  cursor: pointer;
  border-radius: 16px;
}

.button:hover {
  margin-top: 2%;
  background-color: transparent;
  border: solid white 2px;
  color: white;
  font-weight: bold;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  /* display: inline-block; */
  /* margin: 4px 2px; */
  cursor: pointer;
  border-radius: 16px;
}

@media (max-width: 480px) {
  .text-box {
    z-index: 100;
    position: absolute;
    color: white;
    font-size: 24px;
    font-weight: bold;
    top: 20%;
    text-align: center;
    align-items: center;
    width: 100%;
    display: flex;
    flex-direction: column;
}
  .welcome-title{
    font-size: 25px;
    font-weight: bold;
    width: 100%;
  }

  #image {
    height: 400px;
    width: 100%;
    position: relative;
  }
  .typewriter h1 {
  overflow: hidden; /* Ensures the content is not revealed until the animation */
  border-right: .15em solid orange; /* The typwriter cursor */
  white-space: nowrap; /* Keeps the content on a single line */
  margin: 0 auto; /* Gives that scrolling effect as the typing happens */
  letter-spacing: .1em; /* Adjust as needed */
  font-size: 12px;
  animation: 
    typing 2s forwards,
    blink-caret .75s step-end infinite;
}

/* The typing effect */
@keyframes typing {
  from { width: 0 }
  to { width: 100% }
}

/* The typewriter cursor effect */
@keyframes blink-caret {
  from, to { border-color: transparent }
  50% { border-color: orange; }
}


.button {
  margin-top: 2%;
  background-color: white;
  border: solid white 2px;
  color: #8ECAE6;
  font-weight: bold;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  font-size: 14px;
  /* display: inline-block; */
  /* margin: 4px 2px; */
  cursor: pointer;
  border-radius: px;
}
}

</style>