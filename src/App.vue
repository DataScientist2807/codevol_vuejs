<!-- https://github.com/gopinav/Vue-3-Tutorials/blob/master/vue-fundamentals/src/App.vue -->
<template>
  <h2>{{ 2 + 3 + 5 }}</h2>
  <h2>{{ 5 + 10 + 15 }}</h2>
  <h2>Add method - {{ add() }}</h2>
  <h2>Add method - {{ add_new(5,10,15) }}</h2>
  <h2>Multiply method - {{ multiply(baseValue) }}</h2>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      baseMultiplier: 5,
      baseValue: 2
    };
  },
  methods: {
    add(){
      return 2 + 3 + 5
    } ,
    add_new(a,b,c){
      return a + b +c
    },
    multiply(num){
      return num * this.baseMultiplier
    }
  }
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