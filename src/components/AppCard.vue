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
    <img src="" alt="" />
    <h3></h3>
  </div>
</template>

<style scoped lang="scss">
.card {
  height: 100px;
  width: calc(var(--container-size) / 6);
  background-color: red;
  border: 1px solid;
}
</style>
