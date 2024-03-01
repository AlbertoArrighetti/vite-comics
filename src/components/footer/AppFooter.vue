<script>
import AppMerch from './AppMerch.vue';
import AppFooterLinks from './AppFooterLinks.vue';
import AppFooterContacts from './AppFooterContacts.vue';

export default {
  name: 'AppFooter',

  components: {
    AppMerch,
    AppFooterLinks,
    AppFooterContacts,
  }
}

</script>

<template>
    <footer>
        <AppMerch></AppMerch>
        <AppFooterLinks></AppFooterLinks>
        <AppFooterContacts></AppFooterContacts>
    </footer>
</template>

<style lang="scss">

</style>
