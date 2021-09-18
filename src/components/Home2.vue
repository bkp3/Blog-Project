<template>
  <div>
    <h1>Home2 Component</h1>
    <Users/>
    <Products/>
  </div>
</template>
<script>

import Users from './Users'
import Products from './Products'
export default {
  name: "Home2",
  components:{
      Users,
      Products
  }
};
</script>

<style>
div{
    background-color: firebrick;
    height: 500px;
}
</style>