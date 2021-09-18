<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
  <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
  
  <!-- <Home data="You are there" msg="hi from You" /> -->
  <!-- <Home2/> -->
  <!-- <users/> -->
<!-- <Home3/> -->
<Home5/>

</template>

<script>

// import HelloWorld from './components/HelloWorld.vue'
//import Home from "./components/Home.vue";
//import Home2 from './components/Home2.vue';
//import Users from './components/Users.vue';
//import Home3 from './components/Home3.vue';
import Home5 from './components/Home5.vue';

export default {
  name: "App",
  components: {
    // HelloWorld,
    //Home,
    //Home2,
    //Users,
    //Home3,
    Home5
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
