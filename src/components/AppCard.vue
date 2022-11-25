<script>
export default {
  name: "AppCard",
  props: {
    imgSrc: String,
    text: String,
  },
};
</script>

<template>
  <div class="card">
    <div class="image_card">
      <img :src="imgSrc" :alt="text" />
    </div>
    <h3>{{ text }}</h3>
  </div>
</template>

<style scoped lang="scss">
.card {
  width: calc(var(--container-size) / 6);
  display: flex;
  flex-direction: column;
  color: #fff;
  padding: 0 10px;
  .image_card {
    height: 70%;
    overflow: hidden;
  }
  img {
    object-fit: cover;
    width: 100%;
  }
  h3 {
    margin-top: 20px;
  }
}
</style>
