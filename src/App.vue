<script>
import AppNav from './components/AppNav.vue';
import AppMainContent from './components/main/AppMainContent.vue';
import AppFooter from './components/footer/AppFooter.vue';

export default {
  components: {
    AppNav,
    AppMainContent,
    AppFooter,
}
}

</script>

<template>
  <AppNav></AppNav>
  <AppMainContent></AppMainContent>
  
  <AppFooter></AppFooter>
</template>

<style lang="scss">

</style>

