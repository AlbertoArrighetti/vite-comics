<script>
export default {
    name: 'ComicItem',

    props: {
        comicImage: String,
        comicName: String,
        comicType: String,
        comicPrice: String,
    },

    data() {
    },
}
</script>

<template>

    <div class="comic_card">
        <img :src="comicImage" :alt="comicType">
        <span> {{ comicPrice }} </span>
        <h4>{{ comicName }}</h4>
    </div>

</template>

<style lang="scss">
@use '../../styles/variables' as *;

.comic_card {
    width: calc(100% / 6 - 26px / 7 * 6);
    height: 185px;

    margin-bottom: 50px;

    position: relative;

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

    span {
        position: absolute;
        bottom: -26px;
        left: 0;
        font-size: 12px;
        font-family: monospace;
    }
}


</style>