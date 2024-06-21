<template>
  <h2 v-show="showElement">Using v-show</h2>
  <h2 v-if="showElement">Using v-show</h2>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      showElement: false
    };
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