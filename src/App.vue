<template>
 <h2 v-bind:id="headingId">Heading</h2>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
        headingId: 'heading'
          }
  }
}
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