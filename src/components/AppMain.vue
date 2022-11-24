<script>
export default {
  name: 'AppMain',
}
</script>

<template>
  <main>
      <div class="content">
      <div class="container">
        <h2>-->Content goes here..>--</h2>
      </div>
    </div>
    <nav class="info-nav">
            <div class="container">
                <div class="shop-link">
                    <img src="../assets/buy-comics-digital-comics.png" alt="digitalcomics"><a href="#">DIGITAL COMICS</a>
                </div>
                <div class="shop-link">
                    <img src="../assets/buy-comics-merchandise.png" alt="merchandise"><a href="#">DC MERCHANDISE</a>
                </div>
                <div class="shop-link">
                    <img src="../assets/buy-comics-subscriptions.png" alt="subscriptions"><a href="#">SUBSCRIPTION</a>
                </div>
                <div class="shop-link">
                    <img src="../assets/buy-comics-shop-locator.png" alt="shop"><a href="#">COMIC SHOP LOCATOR</a>
                </div>
                <div class="shop-link">
                    <img src="../assets/buy-dc-power-visa.svg" alt="visa"><a href="#">DC POWER VISA </a>
                </div>
            </div>
        </nav>    
  </main>
  
</template>

<style scoped lang="scss">
@import '../style/partials/mixins.scss';
  .content {
    height: 100px;
    background-color: #000;
    @include flexCenter;
      h2 {
        color: #fff;
      }
  }

  .info-nav {
        background-color: var(--primary-color);
        .container {
            display: flex;
            justify-content: space-between ;
            padding: 30px 0;
        }
        .shop-link {
            width: calc(100% / 5);
            @include flexCenter;
            font-size: 1 rem;
                img {
                    width: 50px;
                    margin-right: 10px
                }
                a {
                    text-decoration: none;
                    color:#fff;
                }
        }
    }    
  
</style>