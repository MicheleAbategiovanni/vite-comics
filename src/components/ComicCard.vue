<template>

    <div class="col" v-for="comic, i in comicList">
        <a href="#" class="text-decoration-none text-white ">
            <img :src=comic.thumb :alt=comic.series class="comic-card">
            <h6 class="py-3">{{ comic.series }}</h6>
        </a>
    </div>

</template>

<script>
import { def } from '@vue/shared';


export default {
    props: {
        comicList: Object
  },
}

</script>

<style lang="scss" scoped>

.comic-card {
    aspect-ratio: 1/1;
    width: 100%;
    object-fit: cover;
    object-position: top;
}

</style>