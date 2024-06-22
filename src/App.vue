<!-- https://github.com/gopinav/Vue-3-Tutorials/blob/master/vue-fundamentals/src/App.vue -->
<template>
  <h2>Fullname - {{ firstName }} {{ lastName }}</h2>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      firstName: 'Bruce',
      lastName: 'Wayne'
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