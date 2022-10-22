<template>
  <!-- <nav-bar></nav-bar> -->
  <TestComp></TestComp>
  <router-view/>
</template>

<script>
import TestComp from './components/TestComp.vue';
// import NavBar from './components/global/NavBar.vue';
export default{
  components: {
    // NavBar,
    TestComp
}
}
</script>

<style>
$primary: rebeccapurple;
$danger: #dd0000;
$success: lime;
$warning: orange;
$info: aqua;

$body-bg: #f3f3f0;
html{
  
}

body{
  margin: 0;
  padding: 0;
  font-family: arial,sans-serif;
}

</style>
