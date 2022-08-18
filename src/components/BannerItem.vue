<template>
    <div class="container" id="banner-gallery">
        <div class="banner-card" v-for="(item, index) in bannerMenu" :key="index">
            <a :href="item.url">
                <img :src="item.src" :alt="item.text">
                <p>{{ item.text }}</p>
            </a>
        </div>
    </div>
</template>

<script>
export default {
    name: 'BannerItem',
    props: {
        bannerMenu: Array,
    }
}
</script>

<style lang="scss" scoped>
#banner-gallery {
    padding: 40px 0;
    display: flex;
    justify-content: space-between;
    .banner-card a {
        display: flex;
        align-items: center;
        p {
            margin-left: 10px;
            color: white;
        }
    }
}

</style>