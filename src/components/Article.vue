<template>
  <h2>Article Component</h2>
  <h2>{{ title }}</h2>
</template>

<script>
export default {
    name: 'Article',
    props: {
        title: String
    }
}
</script>

<style>

</style>