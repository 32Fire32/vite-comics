<script>
export default {
  name: 'AppFooter',
}

</script>

<template>
    <footer>
        <nav class="info-nav">
            <div class="container">
                <div class="shop-link">
                    <img src="../assets/buy-comics-digital-comics.png" alt="digitalcomics"><a href="#">Digital Comics</a>
                </div>
                <div class="shop-link">
                    <img src="../assets/buy-comics-merchandise.png" alt="merchandise"><a href="#">Digital Comics</a>
                </div>
                <div class="shop-link">
                    <img src="../assets/buy-comics-subscriptions.png" alt="subscriptions"><a href="#">Digital Comics</a>
                </div>
                <div class="shop-link">
                    <img src="../assets/buy-comics-shop-locator.png" alt="shop"><a href="#">Digital Comics</a>
                </div>
                <div class="shop-link">
                    <img src="../assets/buy-dc-power-visa.svg" alt="visa"><a href="#">Digital Comics</a>
                </div>
            </div>
        </nav>
        <div class="footer-bg">
            <div class="container">
                <div class="footer-links">
                <ul>
                    <li><a href="#">LINK</a></li>
                    <li><a href="#">LINK</a></li>
                    <li><a href="#">LINK</a></li>
                    <li><a href="#">LINK</a></li>
                    <li><a href="#">LINK</a></li>
                    <li><a href="#">LINK</a></li>                 
                </ul>
                </div>
                <div class="big-logo">
                    <img src="../assets/dc-logo-bg.png" alt="logobg">
                </div>
            </div>            
        </div>
        <div class="footer-bottom">
            <div class="container">
                <div class="signup">
                    <button>SIGN-UP NOW!</button>
                </div>
                <div class="social">
                    <h3>FOLLOW US</h3>
                    <img src="../assets/footer-facebook.png" alt="face">
                    <img src="../assets/footer-twitter.png" alt="twit">
                    <img src="../assets/footer-youtube.png" alt="you">
                    <img src="../assets/footer-pinterest.png" alt="pin">
                    <img src="../assets/footer-periscope.png" alt="peri">
                </div>
            </div>
        </div>
        
    </footer>
        
  
</template>

<style scoped lang="scss">

    .info-nav {
        background-color: var(--primary-color);
        .container {
            display: flex;
            justify-content: space-around;
        }
        .shop-link {
            width: calc(100% / 6);
            display: flex;
            align-items: center;
            padding: 20px;
                img {
                    width: 40px;
                }
                a {
                    text-decoration: none;
                    color:#fff;
                }
        }
    }    
    .footer-bg {
        background-image: url(../assets/footer-bg.jpg);
        height: 300px;
        z-index: -2;
        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 100%;
        }
        ul {
            list-style: none;
        }
        a {
            text-decoration: none;
            color:#fff;
        }
        .big-logo {
            z-index: -1;
        }
    }

    .footer-bottom {
        height: 100px;
        background-color:var(--secondary-color);
        display: flex;
        align-items: center;
        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .social {
            display: flex;
        }
    }
</style>