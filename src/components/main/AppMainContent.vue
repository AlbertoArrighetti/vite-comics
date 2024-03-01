<script>

import AppMainGallery from './AppMainGallery.vue';
import AppMerch from './AppMerch.vue';

export default {
    name: 'AppMainContent',
    
    components: {
        AppMainGallery,
        AppMerch,
    } 
}

</script>

<template>
    <main>
        <div class="main_img"></div>
        
        <div class="container">

            <button class="btn_main top">
                Current Series
            </button>
            
            <AppMainGallery></AppMainGallery>

            <button class="btn_main bottom">
                Load More
            </button>
            
        </div>
    </main>
    
    <AppMerch></AppMerch>

    
</template>

<style lang="scss">
@use '../../styles/variables' as *;

@mixin btn_main { 
    background-color: $primaryColor;
    text-transform: uppercase;
    font-weight: bold;
    border: 1px solid $primaryColor;
}

main {
    background-color: #1c1c1c;
    
    

    .main_img {
         background-image: url(/img/jumbotron.jpg);
         height: 400px;
         width: 100%;       
         background-repeat: no-repeat;
         background-size: cover;
    }

    .container {
        padding: 50px 10px 20px;
        flex-direction: column;
        position: relative;

        #gallery {
            margin-bottom: 50px
        }


        .btn_main {
            @include btn_main;
            cursor: pointer;
            
            &.top {
                padding: 16px 30px;
                position: absolute;
                top: -22px;
                left: -20px;
            }

            &.bottom {
                padding: 10px 60px;
            }

            &:hover {
                background-color: white;
                color: $primaryColor;
            }
        }
    }
}
</style>
