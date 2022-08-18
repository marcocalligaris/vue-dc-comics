<template>
    <footer>
        <div class="footer-top">
            <div class="container" id="dc-world">
                <div class="footer-col-left">
                    <div>
                        <h3>DC COMICS</h3>
                        <ul>
                            <li v-for="(item, index) in footerDcComicsMenu" :key="index">
                            <a :href="item.url">{{ item.text }}</a>
                            </li>
                            <h3>SHOP</h3>
                            <ul>
                                <li v-for="(item, index) in footerShopMenu" :key="index">
                            <a :href="item.url">{{ item.text }}</a>
                            </li>
                            </ul>
                        </ul>
                    </div>
                    <div>
                        <h3>DC</h3>
                        <ul>
                            <li v-for="(item, index) in footerDcMenu" :key="index">
                            <a :href="item.url">{{ item.text }}</a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h3>SITES</h3>
                        <ul>
                            <li v-for="(item, index) in footerSitesMenu" :key="index">
                            <a :href="item.url">{{ item.text }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="footer-col-right">
                    <img src="../assets/img/dc-logo-bg.png" alt="DC Comics logo">
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <div class="container">
                <nav>
                    <button type="submit">SIGN-UP NOW!</button>
                    <div id="social-media">
                        <h1>FOLLOW US</h1>
                        <ul>
                            <li v-for="(item, index) in footerSocialMenu" :key="index">
                                <a :href="item.url">
                                    <img :src="(item.src)" :alt="item.text">
                                </a>
                            </li>
                        </ul>
                    </div>
                </nav>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'FooterItem',
    props: {
        footerDcComicsMenu: Array,
        footerShopMenu: Array,
        footerDcMenu: Array,
        footerSitesMenu: Array,
        footerSocialMenu: Array,
    },
}
</script>

<style lang="scss" scoped>
footer {
    color: white;
    height: 600px;
    ul {
        list-style-type: none;
    };
};
.footer-top {
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    height: 80%;
    #dc-world {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;
        .footer-col-left {
            display: flex;
            h3 {
                margin: 15px 0;
            };
            ul li {
                margin-right: 25px;
            };
            ul a {
                color: #878E78;
            };
        };
        .footer-col-right {
            position: relative;
            height: 100%;
            img {
                height: 120%;
                position: relative;
                bottom: -50%;
                transform: translateY(-50%);
            };
        };
    };
};
.footer-bottom {
    background-color: #303030;
    padding: 30px 0;
    height: 20%;
    position: relative;
    left: 0;
    right: 0;
    bottom: 0;
    nav {
        display: flex;
        justify-content: space-between;
        align-items: center;
        button {
            border: solid 2px #0282F9;
            background-color: transparent;
            color: white;
            padding: 10px 20px;
            height: 60px;
            cursor: pointer;
        };
    };
};
.footer-bottom #social-media {
    display: flex;
    align-items: center;
    h1 {
        font-size: 2rem;
        color:#0282F9;
    };
    ul {
        display: flex;
        li {
            margin-left: 20px;
        };
    };
};
</style>