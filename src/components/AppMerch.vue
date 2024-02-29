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

    </section>

</template>

<style lang="scss">
@use '../styles/variables' as *;

 #merch {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 70px;

    padding: 50px 44px;
    background-color: $primaryColor;

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
    }
}

</style>
