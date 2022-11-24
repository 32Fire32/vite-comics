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

  
  
</style>