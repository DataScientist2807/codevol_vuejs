<!-- https://github.com/gopinav/Vue-3-Tutorials/blob/master/vue-fundamentals/src/App.vue -->
 <!-- Computed Properties are cached -->
<template>
 <Portal />
 </template>

<script>
import Portal from './components/Portal.vue'

export default {
  name: "App",
  components: {
    Portal,
  },
  data() {
    return {
      
    };
  },
  methods: {},
  computed: {},
  watch: { },
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