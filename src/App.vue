<template>
  <div id="app">
    <PageHeader />
    <PageMain />
    <CtaList />
    <SocialFoot />   
    <PageFooter />
  </div>
</template>

<script>
import PageHeader from '../../vue-dc-comics/src/components/PageHeader.vue'
import PageMain from '../../vue-dc-comics/src/components/PageMain.vue'
import CtaList from '../../vue-dc-comics/src/components/CtaList.vue'
import SocialFoot from '../../vue-dc-comics/src/components/SocialFoot.vue'
import PageFooter from '../../vue-dc-comics/src/components/PageFooter.vue'

export default {
  name: 'App',
  components: {
    PageHeader,
    PageMain,
    CtaList,
    SocialFoot,
    PageFooter,
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