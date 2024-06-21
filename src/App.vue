<!-- https://github.com/gopinav/Vue-3-Tutorials/blob/master/vue-fundamentals/src/App.vue -->
<template>
  <div>
    <!-- Capture user inputs -->

    <!-- Inputs -->

    <!-- Textareas -->

    <!-- Single select dropdown control -->

    <!-- checkbox -->

    <!-- checkbox group -->

    <!-- radio -->

    <!-- submmit form data -->
  </div>
  


</template>

<script>
export default {
  name: "App",
  data() {
    return {
      name: 'Vishwas',
      count: 0
    };
  },
  methods: {
    changeName(event) {
      this.name = 'Batman'
      console.log('Event', event)
    },
    increment(num, event) {
      this.count += num
      console.log('Event', event)
    },
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