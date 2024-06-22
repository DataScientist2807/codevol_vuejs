<!-- https://github.com/gopinav/Vue-3-Tutorials/blob/master/vue-fundamentals/src/App.vue -->
 <!-- Computed Properties are cached -->
<template>
  <input type="text" v-model="movie">
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      movie: 'Batman'
    };
  },
  methods: {
  },
  computed: {
  },
  watch: {
    /* movie(newValue) {
      console.log(`Calling API with movie name = ${newValue}`)
    } */
    movie: {
      handler(newValue) {
      console.log(`Calling API with movie name = ${newValue}`)
    }
    }
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /*   text-align: center; */
  color: #2c3e50;
  margin-top: 60px;
}

</style>