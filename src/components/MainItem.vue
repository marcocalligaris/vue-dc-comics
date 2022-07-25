<template>
    <main>
        <section id="generic-content">
            <div class="container">
                <h1>--> Content goes here</h1>
            </div>
        </section>
        <section id="links-section">
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

<style scoped>
    main {
        color: white;
    }
    #generic-content {
        padding: 40px 0;
    }
    #links-section {
        height: 200px;
        background-color: #0282F9;
        position: relative;
    }
</style>