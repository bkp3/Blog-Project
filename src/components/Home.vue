<template>
  <div>
    <!-- <h1>This is home component</h1>
    <h2>{{ data }}</h2>
    <h2>{{ msg }}</h2>
    <button v-on:mouseover="hello('hello call')">Call Hello Function</button> -->

    <!-- conditional rendering in vue js -->
    <!-- <h1 v-if="show">conditional rendering in vue js</h1>
    <h1 v-else>conditional rendering else block</h1>
    <button v-on:click="display">Toggle Element</button> -->

    <!-- for loop -->
    <h1>This is for loop example</h1>
    <table>
      <tr>
        <td>Id</td>
        <td>Name</td>
        <td>Email</td>
      </tr>
      <tr v-for="user in users" :key="user.id">
        <td>{{user.id}}</td>
        <td>{{user.name}}</td>
        <td>{{user.email}}</td>
      </tr>
    </table>




  </div>
</template>
<script>
export default {
  name: "Home",
  props: {
    data: String,
    msg: String,
  },
  data() {
    //return { show: true };

    return{
      users:[
        {id:1,name:'Peter',email:'peter@gmail.com'},
        {id:2,name:'Lang',email:'lang@gmail.com'},
        {id:3,name:'Fury',email:'fury@gmail.com'},
        {id:4,name:'Thor',email:'thor@gmail.com'},
      ]
    }

  },
  // methods: {
  //   hello(data) {
  //     alert(data);
  //   },
  //   display(){
  //     this.show=!this.show

  //   },
  // },
};
</script>
