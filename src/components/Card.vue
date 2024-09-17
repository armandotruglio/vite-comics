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
    <div class="container">
        <img :src=imgUrl :alt=comicTitle>
        <h3>{{ comicTitle }}</h3>
    </div>
</template>

<style scoped>
.container {
    max-width: 15%;

    img {
        width: 100%;
    }
}
</style>