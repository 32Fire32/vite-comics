<script>
export default {
  name: 'AppFooter',
}

</script>

<template>
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
</style>