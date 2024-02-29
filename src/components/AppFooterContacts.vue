<script>
export default {
  name: 'AppFooterContacts',

  data() {

    return {
        socialsLogos: [
            '/img/footer-facebook.png',
            '/img/footer-twitter.png',
            '/img/footer-youtube.png',
            '/img/footer-pinterest.png', 
            '/img/footer-periscope.png',
        ],
    }

  },
}
</script>

<template>
    <footer id="footer_contacts">
        <div class="container">
            <div class="btn">
                Sign-up now!
            </div>
    
            <div id="socials">
                <span>
                    follow us
                </span>
                <div id="logos">
                    <div v-for="(currentLogo, index) in socialsLogos">
                        <img :src="currentLogo" alt="">
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss">
@use '../styles/variables' as *;

#footer_contacts{
    background-color: #303030;
    padding: 30px 10px;

    .container {
        justify-content: space-between;

        .btn {
            padding: 14px 12px;
    
            color: white;
            text-transform: uppercase;
            font-weight: bold;
    
            border: 2px solid $primaryColor;
        }
        #socials{
            display: flex;
            align-items: center;
            gap: 26px;

            span {
                text-transform: uppercase;
                color: $primaryColor;
            }
            
            #logos{
                display: flex;
                gap: 18px;
            }
        }
    }
}
</style>
