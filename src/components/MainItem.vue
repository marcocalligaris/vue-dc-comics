<template>
    <main>
        <div id="jumbotron"></div>
        <section>
            <div class="container" id="current-series">
                <div id="series-header">
                <h3>CURRENT SERIES</h3>
                <div id="series-gallery">
                    <div v-for="(item, index) in gallery" :key="index" class="media-card">
                        <a href="#">
                                <img :src="(item.thumb)" :alt="(item.series)">
                                <p>{{ item.series }}</p>
                        </a>
                    </div>
                </div>                
                </div>
                <div class="btn">
                    <button id="load-btn">LOAD MORE</button>
                </div>
            </div>
        </section>
        <section id="banner">
                <BannerItem :bannerMenu="bannerMenu" />
        </section>
    </main>
</template>

<script>
import BannerItem from './BannerItem.vue';
export default {
    name: "MainItem",
    props: {
        gallery: Array,
        bannerMenu: Array,
    },
    components: { BannerItem }
}
</script>

<style lang="scss" scoped>
    #jumbotron {
       background-image: url(../assets/img/jumbotron.jpg);
        background-size: cover;
        height: 400px;
    }
    #current-series {
        position: relative;
        padding-bottom: 30px;
        #series-header {
            h3 {
                display: inline-block;
                padding: 8px 15px;
                color: white;
                background-color: #0282F9;
                position: absolute;
                transform: translateY(-50%);
            };
        };
        #series-gallery {
            display: flex;
            flex-wrap: wrap;
            padding: 30px 0;
            .media-card {
                width: calc(100% / 6);
                padding: 15px;
                img {
                    width: 200px;
                    height: 200px;
                    object-fit: fill;
                    margin-bottom: 20px;
                };
                p {
                    color: white;
                    font-size: 0.9rem;
                    text-transform: uppercase;
                    margin-bottom: 20px;
                }
            };
        };
        .btn {
            display: flex;
            justify-content: center;
            #load-btn {
                color: white;
                font-weight: bold;
                padding: 12px 60px;
                background-color: #0282F9;
            };
        };
    };
    #banner {
        background-color: #0282F9;
        position: relative;
    }
</style>