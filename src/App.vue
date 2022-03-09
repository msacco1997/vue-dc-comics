<template>
  <div id="app">
    <PageHeader />
  </div>
</template>

<script>
import PageHeader from '../../vue-dc-comics/src/components/PageHeader.vue'

export default {
  name: 'App',
  components: {
    PageHeader,
  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family: 'PT Sans Narrow', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>