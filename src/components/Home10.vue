<template>
  <div>
    <h1>Make a form and get data</h1>
    <input
      type="text"
      name="username"
      placeholder="enter your name"
      v-model="loginForm.username"
    /><br /><br />
    <input
      type="password"
      name="password"
      placeholder="enter your password"
      v-model="loginForm.password"
    /><br /><br />
    <button v-on:click="loginData">Login</button>
  </div>
</template>
<script>
export default {
  name: "Home10",
  data() {
    return {
      loginForm: {
        username: null,
        password: null,
      },
    };
  },
  methods: {
    loginData() {
      console.log("loginData",this.loginForm);
    },
  },
};
</script>