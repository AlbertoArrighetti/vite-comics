<script>
export default {
  name: 'AppMerch',

  data() {
    return {
        cards: [
            {
                image: '/img/buy-comics-digital-comics.png',
                text: 'Digital comics',
            },
            {
                image: '/img/buy-comics-merchandise.png',
                text: 'DC Merchandise',
            },
            {
                image: '/img/buy-comics-subscriptions.png',
                text: 'Subscription',
            },
            {
                image: '/img/buy-comics-shop-locator.png',
                text: 'Comic shop locator',
            },
            {
                image: '/img/buy-dc-power-visa.svg',
                text: 'DC Power Visa',
            },
        ]
    }
  },
}

</script>

<template>
    <section id="merch">
        <div class="container">
            <div
            v-for="(cards, index) in cards"
             class="cards">
    
             <div class="img_container">
                 <img :src="cards.image" alt="">
             </div>
             <span>
                 {{ cards.text }}
             </span>
    
            </div>
        </div>

    </section>

</template>

<style lang="scss">
@use '../../styles/variables' as *;

 #merch {
     padding: 50px 10px;
     background-color: $primaryColor;
     
     .container {
         justify-content: center;
         gap: 70px;
         
    }
    .cards{
        display: flex;
        align-items: center;
        gap: 18px;
        
        .img_container{
            height: 56px;
            width: 56px;
            img {
                height: 100%;
                width: 100%;
                object-fit: contain;
            }
        }
        span {
            text-transform: uppercase;
            cursor: pointer;
        }
    }
}

</style>
