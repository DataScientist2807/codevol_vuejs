<!-- https://github.com/gopinav/Vue-3-Tutorials/blob/master/vue-fundamentals/src/App.vue -->
<template>
  <h2>{{ name }}</h2>
  <button @click="name = 'Batman'">Change name</button>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
        name: "Vishwas",
    };
  },
  methods: {
  
  },
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