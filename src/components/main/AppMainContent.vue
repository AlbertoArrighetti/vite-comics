<script>

import AppMainGallery from './AppMainGallery.vue';

export default {
    name: 'AppMainContent',
    
    components: {
        AppMainGallery,
    } 
}

</script>

<template>
    <main>
        <div class="main_img"></div>
        
        <div class="container">
            
            <AppMainGallery></AppMainGallery>
            
        </div>
        

    </main>
</template>

<style lang="scss">
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
        padding: 50px 10px;
    }
}
</style>
