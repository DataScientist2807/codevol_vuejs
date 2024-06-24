<!-- https://github.com/gopinav/Vue-3-Tutorials/blob/master/vue-fundamentals/src/App.vue -->
 <!-- Computed Properties are cached -->
<template>
  <div class="container">
    <div class="content">
      <h1>My App</h1>
      <p>
        sdsadfdsfdsfdsfd
      </p>
      <button @click="showModal = true">Show Modal</button>
      <teleport to="#modal-root">
        <Modal v-show="showModal" @close="showModal = false">This is the secret modal message
        </Modal>
      </teleport>
    </div>
  </div>
 </template>

<script>
import Modal from './components/Modal.vue'

export default {
  name: "App",
  components: {
    Modal,
  },
  data() {
    return {
      showModal: false,
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