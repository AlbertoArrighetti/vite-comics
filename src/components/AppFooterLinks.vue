<script>
export default {
    name: 'AppFooterLinks',

    data() {
      return {
        footerLinks: [
          {
            title: 'DC Comics',
            list: [
              'Characters',
              'Comics',
              'Movies',
              'TV',
              'Games',
              'Videos',
              'News',
            ]
          },
          {
            title: 'Shop',
            list: [
              'Shop DC',
              'Shop DC Collectibles',
            ]
          },
          {
            title: 'DC',
            list: [
              'Terms Of Use',
              'Privacy policy (New)',
              'Ad Choices',
              'Advertising',
              'Jobs',
              'Subscriptions',
              'Talent Workshops',
              'CPSC Certificates',
              'Ratings',
              'Shop Help',
              'Contact Us',
            ]
          },
          {
            title: 'Sites',
            list: [
              'DC',
              'MAD Magazine',
              'DC Kids',
              'DC Universe', 
              'DC Power Visa',
            ]
          },
        ]
      }
    },
}
  

</script>

<template>
  <footer id="footerLinks">
    <div class="container">


      
      <div class="links">
        <div class="list-group" v-for="linkList in footerLinks">
          <h3>{{ linkList.title }}</h3>
          <ul>
            <li v-for="currentLink in linkList.list">
              {{ currentLink }} 
            </li>
          </ul>
        </div>
      </div>
    
    

      <div class="logo">
      </div>
    </div>
  </footer>

</template>

<style lang="scss">
#footerLinks {
  background-image: url(/img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;

  .container {
    justify-content: space-between;
    
    
    .links{
      padding: 40px 0;
      display: flex;
      flex-direction: column;
      flex-wrap: wrap;
      max-height: 400px;
      
      .list-group{
        padding-right: 30px;
        
        h3 {
          margin-bottom: 14px;
          text-transform: uppercase;
        }
        ul {
          list-style-type: none;
          margin-bottom: 18px;
          
          li {
            padding-bottom: 6px;
            opacity: 0.6;
            font-size: 10px;
          }
        }
      }
    }
    
    .logo {
      background-image: url(/img/dc-logo-bg.png);
      background-repeat: no-repeat;
      background-position: center;
      background-size: cover;
      width: 48%;
      height: 400px;
      z-index: 2;
    }
    
  }
  }
</style>
