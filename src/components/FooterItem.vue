<template>
    <footer>
        
        <div class="footer-bottom">
            <div class="container">
                <nav>
                    <button type="submit">SIGN-UP NOW!</button>
                    <div id="social-media">
                        <h1>FOLLOW US</h1>
                        <ul>
                            <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="Facebook"></a></li>
                            <li><a href="#"><img src="../assets/img/footer-twitter.png" alt="Facebook"></a></li>
                            <li><a href="#"><img src="../assets/img/footer-youtube.png" alt="Facebook"></a></li>
                            <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt="Facebook"></a></li>
                            <li><a href="#"><img src="../assets/img/footer-periscope.png" alt="Facebook"></a></li>
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
}
</script>

<style scoped>
footer {
    color: white;
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    height: 600px;
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
    padding: 10px 20px;
    height: 60px;
}

#social-media h1 {
    font-size: 2rem;
    color:#0282F9;
}
.footer-bottom #social-media {
    display: flex;
    align-items: center;
}

#social-media ul {
    list-style-type: none;
    display: flex;
}

#social-media ul li {
    margin-left: 20px;
}
</style>