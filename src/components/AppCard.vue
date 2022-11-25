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
    <img :src="imgSrc" :alt="text" />
    <h3>{{ text }}</h3>
  </div>
</template>

<style scoped lang="scss">
.card {
  height: 100px;
  width: calc(var(--container-size) / 6);
  border: 1px solid;
  display: flex;
  flex-direction: column;
  align-items: center;
  img {
    object-fit: cover;
    height: 100%;
  }
}
</style>
