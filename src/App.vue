<template>
  <h2 v-if="num === 0">The number is zero</h2>
  <h2 v-if="num === 2">The number is two</h2>
  <h2 v-else-if="num > 3">The number is greater than two</h2>
  <h2 v-else-if="num <= 2">The number is less or equal than two</h2>
  <h2 v-else>The number is three</h2>
  <div v-if="display">
    <h2>Vishwas</h2>
    <h2>Codevolution</h2>
    <h2>Vue</h2>
  </div>
  <hr>
  <template v-if="display">
    <h2>Vishwas</h2>
    <h2>Codevolution</h2>
    <h2>Vue</h2>
  </template>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      num: 3,
      display: true
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