<template>
    <div>
        <div class="footer-top">
            <div class="container">
        
            </div>
        </div>
        <div class="footer-bottom">
            <div class="container">
                <nav>
                    <button type="submit">SIGN-UP NOW!</button>
                </nav>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FooterItem',
}
</script>

<style scoped>
footer {
    color: white;
}
.footer-bottom {
    background-color: #303030;
    padding: 30px 0;
}
.footer-bottom nav {
    display: flex;
    justify-content: space-between;
}
.footer-bottom nav button {
    border: solid 2px #0282F9;
    background-color: transparent;
    color: white;
    padding: 10px;
}
</style>