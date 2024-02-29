<script>
export default {
    name: 'AppNav',
  data() {
    return {
      links: [
        'Characters',
        'Comics',
        'Movies',
        'Tv',
        'Games',
        'Collectibles',
        'Videos',
        'Fans',
        'News',
        'Shop',
      ]
    }
  }
}
</script>



<template>
  <nav>
    <img id="logo" src="/img/dc-logo.png" alt="Logo DC">
    <ul id="links">
      <li v-for="(currentLink, index) in links">
        {{ currentLink }}
      </li>
    </ul>
  </nav>
</template>



<style lang="scss">
@use '../styles/variables' as *;

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 10px;

  background-color: #ffffff;
  color: black;

  #logo{
    width: 84px;
    height: auto;
  }
  #links{
    display: flex;
    margin: 0;
    gap: 30px;

    list-style-type: none;
    li{
      padding: 50px 0;
      font-weight: 500;
      text-transform: uppercase;
      cursor: pointer;

      &:hover{
        color: $primaryColor;
        padding: calc(50px - 4px) 0;
        border-bottom: 4px solid $primaryColor;
      }
    }

  }
}
</style>
