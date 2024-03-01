<script>
export default {
    name: 'ComicItem',

    props: {
        comicImage: String,
        comicName: String,
        comicType: String,
    },

    data() {
    },
}
</script>

<template>

    <div class="comic_card">
        <img :src="comicImage" :alt="comicType">
        <h4>{{ comicName }}</h4>
    </div>

</template>

<style lang="scss">

.comic_card {
    width: calc(100% / 6 - 26px / 7 * 6);
    height: 185px;

    margin-bottom: 50px;

    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: top;

        margin-bottom: 20px;
    }

    h4 {
        text-transform: uppercase;
        font-weight: 400;
        font-size: 12px;
    }
}


</style>