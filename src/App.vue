<!-- https://github.com/gopinav/Vue-3-Tutorials/blob/master/vue-fundamentals/src/App.vue -->
 <!-- Computed Properties are cached -->
<template>
   <Article title="Article Title"/>
 </template>

<script>
import Article from './components/Article.vue'

export default {
  name: "App",
  components: {
    Article,
  },
  data() {
    return {
      name: 'Vishwas',
      channel: 'Codevolution'
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
  /*   text-align: center; */
  color: #2c3e50;
  margin-top: 60px;
}
</style>