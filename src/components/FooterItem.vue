<template>
    <footer>
        <div class="footer-top">
            <div class="container" id="dc-world">
                <div class="footer-col-left">
                    <div>
                        <h3>DC COMICS</h3>
                        <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                            <h3>SHOP</h3>
                            <ul>
                                <li><a href="#">Shop DC</a></li>
                                <li><a href="#">Shop DC Collectibles</a></li>
                            </ul>
                        </ul>
                    </div>
                    <div>
                        <h3>DC</h3>
                        <ul>
                            <li><a href="#">Terms Of Use</a></li>
                            <li><a href="#">Privacy policy (New)</a></li>
                            <li><a href="#">Ad Choices</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscriptions</a></li>
                            <li><a href="#">Talent Workshops</a></li>
                            <li><a href="#">CPSC Certificates</a></li>
                            <li><a href="#">Ratings</a></li>
                            <li><a href="#">Shop Help</a></li>
                            <li><a href="#">Contact Us</a></li>
                        </ul>
                    </div>
                    <div>
                        <h3>SITES</h3>
                        <ul>
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
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
    height: 600px;
}

.footer-top {
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    height: 80%;
}

footer ul {
    list-style-type: none;
}

.footer-top #dc-world {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100%;
}

.footer-top #dc-world .footer-col-left {
    display: flex;
}

.footer-col-left h3 {
    margin: 15px 0;
}

.footer-col-left ul li {
    margin-right: 25px;
}

.footer-col-left ul a {
    color: #878E78;
}

.footer-top #dc-world .footer-col-right {
    position: relative;
    height: 100%;
}

.footer-col-right img {
    height: 120%;
    position: relative;
    bottom: -50%;
    transform: translateY(-50%);
}
.footer-bottom {
    background-color: #303030;
    padding: 30px 0;
    height: 20%;
    position: relative;
    left: 0;
    right: 0;
    bottom: 0;
}
.footer-bottom nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
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
    display: flex;
}

#social-media ul li {
    margin-left: 20px;
}
</style>