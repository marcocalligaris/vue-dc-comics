<template>
    <header>
        <div class="container">
            <figure>
                <a href="#"><img src="../assets/img/dc-logo.png" alt="DC Comics logo"></a>
            </figure>
            <nav>
                <ul>
                    <li><a href="#">CHARACTERS</a></li>
                    <li><a href="#" class="active">COMICS</a></li>
                    <li><a href="#">MOVIES</a></li>
                    <li><a href="#">TV</a></li>
                    <li><a href="#">GAMES</a></li>
                    <li><a href="#">COLLECTIBLES</a></li>
                    <li><a href="#">VIDEOS</a></li>
                    <li><a href="#">FANS</a></li>
                    <li><a href="#">NEWS</a></li>
                    <li><a href="#">SHOP</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'HeaderItem',
}
</script>

<style scoped>
    header {
        background-color: #fff;
        height: 100px;
    }
    header .container {
        height: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    header figure img {
        display: block;
    }

    header nav ul {
        display: flex;
    }
    header ul li {
        line-height: 100px;
        margin-left: 30px;
    }

    header ul li:hover {
        box-shadow: 0px -4px 0px #0282F9 inset;
    }

    header ul a {
        font-size: 12px;
        font-weight: bold;
        transition: color 0.3s;
    }

    header ul a.active,
    header ul a:hover {
        color: #0282F9;
    }
</style>