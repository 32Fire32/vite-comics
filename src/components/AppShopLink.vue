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
  <div class="image">
    <img :src="imgSrc" :alt="shopText" />
  </div>
  <h3>{{ shopText }}</h3>
</template>

<style scoped lang="scss">
img {
  width: 30px;
  margin-right: 10px;
  display: block;
}
</style>
