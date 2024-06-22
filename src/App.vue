<!-- https://github.com/gopinav/Vue-3-Tutorials/blob/master/vue-fundamentals/src/App.vue -->
 <!-- Computed Properties are cached -->

<template>
  <h2>{{ fullname }}</h2>
<button @click="changeFullName">Change Fullname</button>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      fullname: 'Bruce Wayne'
    };
  },
  methods: {
    changeFullName() {
      this.fullname = 'Clark Kent'
    }
  },
  computed: {
    fullName: {
      get() {
        return `${this.firstName} ${this.lastName}`
      },
      set(value) {
        const names = value.split('')
        this.firstName = names[0]
        this.lastName = names[1]

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