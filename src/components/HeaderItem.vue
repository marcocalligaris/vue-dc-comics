<template>
    <header>
        <div class="container">
            <figure>
                <a href="#"><img src="../assets/img/dc-logo.png" alt="DC Comics logo"></a>
            </figure>
            <nav>
                <ul>
                    <li v-for="link in links" :key="link.id">
                        <a
                            :href="link.url"
                            :class="{'active': link.active }"
                            >
                            {{ link.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'HeaderItem',
    props: {
        links: Array,
    }
}
</script>

<style lang="scss" scoped>
    header {
        background-color: #fff;
        height: 100px;
        .container {
            height: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        figure img {
            display: block;
        }
        nav ul {
            display: flex;
            li {
                line-height: 100px;
                margin-left: 30px;
            }
            li:hover {
                box-shadow: 0px -4px 0px #0282F9 inset;
            }
            a {
                font-size: 12px;
                font-weight: bold;
                transition: color 0.3s;
            }
            a.active,
            a:hover {
                color: #0282F9;
            }
        }
    }
</style>