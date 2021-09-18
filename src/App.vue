<template>
  <div>
    <h1 style="color:red;"><u>Welcome to Vue.js World</u></h1>
    <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
    <!-- <HelloWorld msg="Welcome to Vue.js hello World" /> -->

    <!-- <Home data="You are there" msg="hi from You" /> -->
    <!-- <Home2/> -->
    <!-- <users/> -->
    <!-- <Home3/> -->
    <!-- <Home6 v-bind:users="users"/> -->
    <h2>{{title}}</h2>
    <Home7 v-on:changeTitle="changeTitle($event)"/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
//import Home from "./components/Home.vue";
//import Home2 from './components/Home2.vue';
//import Users from './components/Users.vue';
//import Home3 from './components/Home3.vue';
import Home7 from "./components/Home7.vue";

export default {
  name: "App",
  components: {
    // HelloWorld,
    //Home,
    //Home2,
    //Users,
    //Home3,
    Home7,
  },
  // data(){
  //     return{
  //       users:[
  //         {name:"peter",email:"peter@gmail.com"},
  //         {name:"harry",email:"harry@gmail.com"},
  //         {name:"rocky",email:"rocky@gmail.com"},
  //         {name:"mak",email:"mak@gmail.com"},
  //       ]
  //     }
  // }

  data(){
    return{
      title:"props tutorial"
    }
  },
  methods:{
    changeTitle(title){ 
      this.title=title
    }
  }
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
