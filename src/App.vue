<!-- https://github.com/gopinav/Vue-3-Tutorials/blob/master/vue-fundamentals/src/App.vue -->
<template>
  <h2>{{ name }}</h2>
  <div>
    <button v-on:click="name = 'Batman'">Change name</button>
    <hr />
    <button v-on:mouseover="name = 'Batman over'">Change name</button>
  </div>
  <h2>{{ count }}</h2>
  <div>
    <!-- <button v-on:click="count = count + 1">Increment</button>
    <button v-on:click="count = count - 1">Decrement</button> -->
    <!-- <button v-on:click="increment">Increment</button>
    <button v-on:click="decrement">Decrement</button> -->
    <button v-on:click="increment(1)">Increment</button>
    <button v-on:click="increment(5)">Decrement</button>
    <button v-on:click="decrement(1)">Increment</button>
    <button v-on:click="decrement(5)">Decrement</button>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      name: "Vishwas",
      count: 0,
    };
  },
  methods: {
    /* increment() {
      this.count += 1;
    },
    decrement() {
      this.count -= 1;
    }, */
    increment(num) {
      this.count += num;
    },
    decrement(num) {
      this.count -= num;
    },
  },
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