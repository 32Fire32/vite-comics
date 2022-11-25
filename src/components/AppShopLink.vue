<script>
export default {
  name: "AppShopLink",
  props: {
    imgSrc: String,
    shopText: String,
  },
};
</script>

<template>
  <div class="shop">
    <div class="image">
      <img :src="imgSrc" :alt="shopText" />
    </div>
    <h3>{{ shopText }}</h3>
  </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins.scss" as *;
.shop {
  width: calc(var(--container-size) / 5);
  @include flexCenter;
  justify-content: center;
  img {
    width: 50px;
    margin-right: 10px;
    display: block;
  }
}
</style>
