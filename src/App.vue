<!-- https://github.com/gopinav/Vue-3-Tutorials/blob/master/vue-fundamentals/src/App.vue -->
<template>
  <h2>Fullname - {{ firstName }} {{ lastName }}</h2>
  <h2>Fullname - {{ fullName }}</h2>
  <h2>Total - {{ items.reduce((total, curr) => (total = total + curr.price), 0)}}</h2>
  <h2>Computed Total - {{ total }}</h2>
  <h2>Method Total - {{ getTotal() }}</h2>
<input type="text" v-model="country">
<button @click="items.push({id: 4, title: 'Phone', price: 50, })">Add item</button>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      firstName: 'Bruce',
      lastName: 'Wayne',
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
      country: ''
    };
  },
  methods: {
    getTotal() {
      console.log('getTotal Method')
      return this.items.reduce((total, curr) => (total = total + curr.price), 0)
    }
  },
  computed: {
    fullName() {
      return `${this.firstName} ${this.lastName}`
    },
    total() {
      console.log('total computed property')
      return this.items.reduce((total, curr) => (total = total + curr.price), 0)
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