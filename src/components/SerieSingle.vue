<template>
    <figure>
        <div>
            <img :src="serieSrc" :alt="serieTitle">
        </div>
        <figcaption>{{ serieTitle }}</figcaption>
    </figure>
</template>

<script>
export default {
    name: 'SerieSingle',
    props: {
        serieSrc: String,
        serieTitle: String,
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/sass/vars';

figure {
    font-size: 14px;
    text-transform: uppercase;

    div {
        height: 180px;
        overflow-y: hidden;

        img {
            width: 100%;
        }
    }

    figcaption {
        padding: 15px 0;
        text-align: left;
    }
}
</style>