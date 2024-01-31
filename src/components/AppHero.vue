<script>
export default {
    name: 'AppHero',
    data: () => ({
        image_name: 'zororandom2.jpg'
    }),
    methods: {
        createImagePath(image_name) {

            const url = new URL(`../assets/${image_name}`, import.meta.url)
            return url.href
        }
    }
}
</script>


<template>
    <div class="jumbotron">
        <img src="../../public/zororandom.jpg" alt="Zoro1">
        <img :src="createImagePath(image_name)" alt="Zoro2">
    </div>
</template>


<style>
img {
    max-width: 500px;
    height: auto;
    padding-top: 20px;
}
</style>