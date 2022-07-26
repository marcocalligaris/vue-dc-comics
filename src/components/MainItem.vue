<template>
    <main>
        <div id="jumbotron"></div>
        <section>
            <div class="container" id="current-series">
                <div>
                <h3>CURRENT SERIES</h3>
                </div>
                <h1>--> Content goes here</h1>
            </div>
        </section>
        <section id="banner">
            <div class="container">
                <nav>
                    <ul>
                        <li></li>
                    </ul>
                </nav>
            </div>
        </section>
    </main>
</template>

<script>
export default {
    name: 'MainItem',
}
</script>

<style lang="scss" scoped>
    main {
        color: white;
        #jumbotron {
            background-image: url(../assets/img/jumbotron.jpg);
            background-size: cover;
            height: 400px;
        }

    }


    #banner {
        padding: 40px 0;
        height: 150px;
        background-color: #0282F9;
        position: relative;
    }
</style>