<script>
export default {
  name: 'AppFooter',
  data() {
      return {
         dcComics: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News' ],
         shops: ['Shop DC', 'Shop DC Collectibles'],
         others:['Terms Of Use', 'Privacy policy(New)', 'Ad Choices', 'Advertising', 'Jobs', 'Subscriptions', 'Talent Workshops', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us'],
         sites:['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa']

      }
    }
}



</script>

<template>
    <footer>
        <div class="footer-bg">
            <div class="container">
                <div class="footer-links">
                    <div class="links">
                        <h3>DC COMICS</h3>
                        <ul>
                            <li v-for="comic in dcComics"><a href="#">{{ comic }}</a></li>               
                        </ul>
                        <h3>SHOP</h3>
                        <ul>
                            <li v-for="shop in shops"><a href="#">{{ shop }}</a></li>               
                        </ul>
                    </div>
                    <div class="links">
                        <h3>DC</h3>
                        <ul>
                            <li v-for="other in others"><a href="#">{{ other }}</a></li>               
                        </ul>
                    </div>
                    <div class="links">
                        <h3>SITES</h3>
                        <ul>
                            <li v-for="site in sites"><a href="#">{{ site }}</a></li>               
                        </ul>
                    </div>              
                </div>
                    <img src="../assets/dc-logo-bg.png" alt="logobg">
            </div>            
        </div>
        <div class="footer-bottom">
            <div class="container">
                    <button>SIGN-UP NOW!</button>
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
        img {
            width: 50%;
        }
        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 100%;
            position: relative;
            .footer-links {
                display: flex;
                .links {
                    padding: 10px;
                }
            }
            img {
                width: 30%;
                position: absolute;
                right: 0;
                }        
        }

        h3 {
            color: #fff;
            margin: 10px 0;
        }

        ul {
            list-style: none;
        }

        a {
            text-decoration: none;
            color:gray;
            font-size: 14px;
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
            button {
                border: 1px solid var(--primary-color);
                background-color: var(--secondary-color);
                padding: 10px;
                color: #fff;
            }
        }
        .social {
            display: flex;
            h3 {
                color: var(--primary-color),
            }
            img {
                margin-left: 10px;
            }
        }
    }
</style>