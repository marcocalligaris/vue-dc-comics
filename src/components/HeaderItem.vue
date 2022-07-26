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
    data(){
        return {
            links:[
                {id:1, url:'#', text:'CHARACTERS', active: false},
                {id:2, url:'#', text:'COMICS', active: false},
                {id:3, url:'#', text:'MOVIES', active: false},
                {id:4, url:'#', text:'TV', active: false},
                {id:5, url:'#', text:'GAMES', active: false},
                {id:6, url:'#', text:'COLLECTIBLES', active: false},
                {id:7, url:'#', text:'VIDEOS', active: false},
                {id:8, url:'#', text:'FANS', active: false},
                {id:9, url:'#', text:'NEWS', active: false},
                {id:10, url:'#', text:'SHOP', active: false},
            ]
        }
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