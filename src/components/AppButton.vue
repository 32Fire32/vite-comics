<script>
export default {
  name: "AppButton",
};
</script>

<template>
  <button>CURRENT SERIES</button>
</template>

<style scoped lang="scss">
button {
  @include btn;
  font-weight: bolder;
  position: absolute;
  top: -18px;
  left: 0;
}
</style>
