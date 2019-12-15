<template>
  <div class="heroImage"></div>
</template>

<script>
export default {
  name: 'HeroImage',
};
</script>
<style lang="scss" scoped>
  .heroImage {
    position: fixed;
    width: 100%;
    height: 100vh;
    z-index: -1;
    top: 0;
    background-image: url('../assets/heroimage.jpg');
    background-repeat: no-repeat;
    background-position: 80% 0%;
    background-size: cover;

    &::after {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      z-index: 1;
      width: 100%;
      height: 100vh;
      background: rgba(0,0,0, .2);
    }
  }
</style>
