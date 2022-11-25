<script>
import AppBlue from "./AppBlue.vue";
export default {
  name: "AppHeader",
  components: {
    AppBlue,
  },

  data() {
    return {
      navLinks: [
        {
          link: "CHARACTERS",
          active: false,
        },
        {
          link: "COMICS",
          active: false,
        },
        {
          link: "MOVIES",
          active: false,
        },
        {
          link: "TV",
          active: false,
        },
        {
          link: "GAMES",
          active: false,
        },
        {
          link: "COLLECTIBLES",
          active: false,
        },
        {
          link: "VIDEO",
          active: false,
        },
        {
          link: "FANS",
          active: false,
        },
        {
          link: "NEWS",
          active: false,
        },
        {
          link: "SHOP",
          active: false,
        },
      ],
    };
  },
  methods: {
    changeButton(index) {
      this.navLinks.forEach((elm, i) => {
        if (i === index) {
          elm.active = true;
        } else {
          elm.active = false;
        }
      });
    },
  },
};
</script>

<template>
  <header>
    <div class="container">
      <div class="logo">
        <img src="../assets/dc-logo.png" alt="dcLogo" />
      </div>
      <nav>
        <AppBlue />
        <ul class="nav_header">
          <li v-for="(link, index) in navLinks">
            <a
              href="#"
              :class="{ active: link.active }"
              @click.prevent="changeButton(index)"
              >{{ link.link }}</a
            >
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<style scoped lang="scss">
@import "../style/partials/mixins.scss";

header {
  padding: 10px;
}
.container {
  @include flexCenter;
  justify-content: space-between;
  img {
    width: 50px;
  }
}
nav {
  position: relative;
  .active {
    color: var(--primary-color);
  }
}

ul {
  display: flex;

  li {
    position: relative;
    list-style: none;
    margin: 0 20px;
    color: var(--secondary-color);
    font-weight: bold;
    font-size: 10px;
    a {
      text-decoration: none;
      color: inherit;
    }
  }
}
</style>
