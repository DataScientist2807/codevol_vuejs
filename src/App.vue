<template>
    <h2 v-bind:style="{ color: highlightColor}">Inline Style</h2>
    <h2 v-bind:style="{ color: highlightColor, 'font-size': headerSize + 'px' }">Inline Style</h2>
    <h2 v-bind:style="{ color: highlightColor, fontSize: headerSize + 'px' }">Inline Style</h2>
    <h2 v-bind:style="{ color: highlightColor, fontSize: headerSize + 'px', padding: '20px' }">Inline Style</h2>
    <h2 v-bind:style="headerStyleObject">Header Style Object</h2>
    <h2 v-bind:style="[headerStyleObject, successStyleObject]">Combined Style Object</h2>
    <h2 v-bind:style="[headerStyleObject, dangerStyleObject]">Danger Combined Style Object</h2>

</template>

<script>
export default {
  name: "App",
  data() {
    return {
      highlightColor: 'orange',
      headerSize: 50,
      headerStyleObject: {
        color: 'blue',
        fontSize: '50px',
        padding: '20px'
      },
      successStyleObject: {
        color: 'green',
        fontSize: '20px',
        padding: '10px'
      },
      dangerStyleObject: {
        color: 'red',
        fontSize: '20px',
        padding: '10px'
      }
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

</style>