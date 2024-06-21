<template>
    <h2 class="underline">Underlined text</h2>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      headingId: "heading",
      isDisabled: false,
      enabled: true
    };
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
.underline {
  text-decoration: underline;
}
</style>