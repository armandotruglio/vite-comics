<script>
export default {
    data() {
        return {
        }
    },
    props: {
        imgUrl: {
            type: String,
            required: true
        },
        comicTitle: {
            type: String,
            required: true,
        }
    }
}
</script>

<template>
    <div class="card">
        <figure>
            <img :src=imgUrl :alt=comicTitle>
        </figure>
        <h3>{{ comicTitle }}</h3>
    </div>
</template>

<style lang="scss" scoped>
.card {
    flex-basis: calc(100%/6 - 30px);

    figure {
        height: 180px;
        overflow-y: hidden;

        img {
            width: 100%;
        }
    }

    h3 {
        font-size: 0.8rem;
        font-weight: lighter;
        text-transform: uppercase;
        margin-top: 1rem;
    }
}
</style>