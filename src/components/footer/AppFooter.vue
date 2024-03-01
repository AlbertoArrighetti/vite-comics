<script>

import AppFooterLinks from './AppFooterLinks.vue';
import AppFooterContacts from './AppFooterContacts.vue';

export default {
  name: 'AppFooter',

  components: {
    AppFooterLinks,
    AppFooterContacts,
  }
}

</script>

<template>
    <footer>
        <AppFooterLinks></AppFooterLinks>
        <AppFooterContacts></AppFooterContacts>
    </footer>
</template>

<style lang="scss">

</style>
