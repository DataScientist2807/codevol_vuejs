<template>
    <h2 class="underline">Underlined text</h2>
    <h2 v-bind:class="status">Status</h2>
    <h2 class="underline" v-bind:class="status">Status</h2>
    <h2 v-bind:class="isPromoted && 'promoted'">Promoted Movie</h2>
    <h2 v-bind:class="isNotPromoted && 'promoted'">Promoted Movie</h2>
    <h2 v-bind:class="isSoldout ? 'sold-out' : 'new'">Soldout? Movie</h2>
    <h2 v-bind:class="['new', 'promoted']">Newly promoted Movie</h2>
    <h2 v-bind:class="[isPromoted && 'promoted', isSoldout ? 'sold-out' : 'new']">Array conditional Movie</h2>
    <h2 :class="{promoted: isPromoted, new: !isSoldout, 'sold-out': isSoldout,}">Object Conditional Movie</h2>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      status: 'danger',
      isPromoted: false,
      isNotPromoted: false,
      isSoldout: false
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
.promoted {
  font-style: italic;
}
.new {
  color: olivedrab;
}
.sold-out {
  color: red;
}
</style>