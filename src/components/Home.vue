<template>
  <div>
    <h1>This is home component</h1>
    <h2>{{ data }}</h2>
    <h2>{{ msg }}</h2>
    <button v-on:mouseover="hello('hello call')">Call Hello Function</button>
    

  </div>
</template>
<script>
export default {
  name: "Home",
  props: {
    data: String,
    msg: String,
  },
  methods: {
    hello(data) {
      alert(data)
    },
  },
};
</script>
