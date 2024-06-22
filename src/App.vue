<!-- https://github.com/gopinav/Vue-3-Tutorials/blob/master/vue-fundamentals/src/App.vue -->
 <!-- Computed Properties are cached -->
<template>
  <input type="text" v-model="movie" />
  <input type="text" v-model="movieInfo.title" />
  <input type="text" v-model="movieInfo.actor" />
<div>
  <button @click="movieList.push('Wonder Woman')">Add movie</button>
</div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      movie: "Batman2",
      movieInfo: {
        title: '',
        actor: ''
      },
      movieList: ['Batman', 'Superman']
    };
  },
  methods: {},
  computed: {},
  watch: {
    movie: {
      handler(newValue) {
        console.log(`Calling API with movie name = ${newValue}`);
      },
      immediate: true,
    },
    movieInfo: {
      handler(newValue) {
        console.log(`Calling API with movie title = ${newValue.title} and actor = ${newValue.actor}`);
      },
      deep: true,
    },
    movieList: {
      handler(newValue) {
        console.log(`Updated list ${newValue}`)
      },
      deep: true,
    }
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