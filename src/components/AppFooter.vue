<script>
export default {
  name: 'AppFooter',
}

</script>

<template>
    <footer>
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
                    <img src="../assets/dc-logo-bg.png" alt="logobg">
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
    
    .footer-bg {
        background-image: url(../assets/footer-bg.jpg);
        height: 300px;
        img {
            width: 50%;
        }
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
    }

    .footer-bottom {
        z-index: 100;
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