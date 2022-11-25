<script>
import AppShopLink from "./AppShopLink.vue";
export default {
  name: "AppFooter",
  components: {
    AppShopLink,
  },

  data() {
    return {
      shopLinks: [
        {
          img: "src/assets/buy-comics-digital-comics.png",
          text: "DIGITAL COMICS",
        },
        {
          img: "src/assets/buy-comics-merchandise.png",
          text: "DC MERCHANDISE",
        },
        {
          img: "src/assets/buy-comics-subscriptions.png",
          text: "SUBSCRIPTIONS",
        },
        {
          img: "src/assets/buy-comics-shop-locator.png",
          text: "COMIC SHOP LOCATOR",
        },
        {
          img: "src/assets/buy-dc-power-visa.svg",
          text: "DC POWER VISA",
        },
      ],

      dcComics: [
        "Characters",
        "Comics",
        "Movies",
        "TV",
        "Games",
        "Videos",
        "News",
      ],
      shops: ["Shop DC", "Shop DC Collectibles"],
      others: [
        "Terms Of Use",
        "Privacy policy(New)",
        "Ad Choices",
        "Advertising",
        "Jobs",
        "Subscriptions",
        "Talent Workshops",
        "CPSC Certificates",
        "Ratings",
        "Shop Help",
        "Contact Us",
      ],
      sites: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],
    };
  },
};
</script>

<template>
  <footer>
    <nav class="info-nav">
      <div class="container">
        <div class="shop-link" v-for="shop in shopLinks">
          <AppShopLink :imgSrc="shop.img" :shopText="shop.text" />
        </div>
      </div>
    </nav>
    <div class="footer-bg">
      <div class="container">
        <div class="footer-links">
          <div class="links">
            <h3>DC COMICS</h3>
            <ul>
              <li v-for="comic in dcComics">
                <a href="#">{{ comic }}</a>
              </li>
            </ul>
            <h3>SHOP</h3>
            <ul>
              <li v-for="shop in shops">
                <a href="#">{{ shop }}</a>
              </li>
            </ul>
          </div>
          <div class="links">
            <h3>DC</h3>
            <ul>
              <li v-for="other in others">
                <a href="#">{{ other }}</a>
              </li>
            </ul>
          </div>
          <div class="links">
            <h3>SITES</h3>
            <ul>
              <li v-for="site in sites">
                <a href="#">{{ site }}</a>
              </li>
            </ul>
          </div>
        </div>
        <div class="logoBg">
          <img src="../assets/dc-logo-bg.png" alt="logobg" />
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <div class="container">
        <button>SIGN-UP NOW!</button>
        <div class="social">
          <h3>FOLLOW US</h3>
          <img src="../assets/footer-facebook.png" alt="face" />
          <img src="../assets/footer-twitter.png" alt="twit" />
          <img src="../assets/footer-youtube.png" alt="you" />
          <img src="../assets/footer-pinterest.png" alt="pin" />
          <img src="../assets/footer-periscope.png" alt="peri" />
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped lang="scss">
.info-nav {
  position: relative;
  z-index: 2;
  background-color: var(--primary-color);
  .container {
    display: flex;
    justify-content: space-between;
    padding: 30px 0;
    .shop-link {
      color: #fff;
      @include flexCenter;
    }
  }
}
.footer-bg {
  background-image: url(../assets/footer-bg.jpg);
  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100%;
    position: relative;
    img {
      right: 0;
      top: -60px;
      width: 30%;
      position: absolute;
    }
    .footer-links {
      display: flex;
      .links {
        padding: 10px;
      }
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
    color: gray;
    font-size: 14px;
  }
}

.footer-bottom {
  position: relative;
  height: 100px;
  background-color: var(--secondary-color);

  @mixin flexCenter {
    display: flex;
    align-items: center;
  }
  @include flexCenter;
  .container {
    @include flexCenter;
    justify-content: space-between;
    width: 100%;

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
      color: var(--primary-color);
    }
    img {
      margin-left: 10px;
    }
  }
}
</style>
