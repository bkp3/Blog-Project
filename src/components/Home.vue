<template>
  <div>
    <h1>This is home component</h1>
    <h2>{{ data }}</h2>
    <h2>{{ msg }}</h2>
    <button v-on:mouseover="hello('hello call')">Call Hello Function</button>

    <!-- conditional rendering in vue js -->
    <h1 v-if="show">conditional rendering in vue js</h1>
    <h1 v-else>conditional rendering else block</h1>
    <button v-on:click="display">Toggle Element</button>
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
    return { show: true };
  },
  methods: {
    hello(data) {
      alert(data);
    },
    display(){
      this.show=!this.show

    },
  },
};
</script>
