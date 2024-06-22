<!-- https://github.com/gopinav/Vue-3-Tutorials/blob/master/vue-fundamentals/src/App.vue -->
 <!-- Computed Properties are cached -->
<template>
  <Greet name="Bruce" heroName="Batman"/>
  <Greet name="Clark" heroName="Superman"/>
  <Greet name="Diana" heroName="Wonder Woman"/>
  <Greet :name="name" :heroName="channel"/>

</template>

<script>
import Greet from './components/Greet.vue'
export default {
  name: "App",
  components: {
    Greet,
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