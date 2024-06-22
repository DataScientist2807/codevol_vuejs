<!-- https://github.com/gopinav/Vue-3-Tutorials/blob/master/vue-fundamentals/src/App.vue -->
 <!-- Computed Properties are cached -->
  
<template>
 <template v-for="item in items" :key="item.id">
  <h2 v-if="item.price > 100">{{ item.title }} {{ item.price }}</h2>
 </template>
 <h2 v-for="item in expensiveItems" :key="item.title">{{ item.title }} {{ item.price }}</h2>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      items: [
        {
          id: 1,
          title: 'TV',
          price: 100,
        },
        {
          id: 2,
          title: 'Phone',
          price: 200,
        },
        {
          id: 3,
          title: 'Laptop',
          price: 300,
        },
      ],
    };
  },
  methods: {
    
  },
  computed: {
    expensiveItems() {
      return this.items.filter( item => item.price > 100)
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