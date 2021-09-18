<template>
  <div>
    <h1>life cycle methods (Hooks)</h1>
  </div>
</template>
<script>
export default {
  name: "Home8",
  beforeCreate: function () {
    console.warn("beforeCreated");
  },
  created: function () {
    console.warn("created");
  },

  beforeMount: function () {
    console.warn("beforeMount");
  },
  mounted: function () {
    console.warn("mounted");
  },
};
</script>