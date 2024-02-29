<script>
import AppNav from './components/AppNav.vue';
import AppMainContent from './components/AppMainContent.vue';
import AppFooter from './components/AppFooter.vue';

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

// container in comune
.container {
  max-width: 1300px;
  margin: 0 auto;

  display: flex;
  align-items: center;
}
</style>

