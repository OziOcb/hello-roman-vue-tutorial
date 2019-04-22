<template>
  <div class="heroImage"></div>
</template>

<script>
export default {
  name: 'HeroImage',
}
</script>

<style lang="scss" scoped>
  .heroImage {
    width: 100%;
    height: 100vh;
    position: fixed;
    top: 0;
    z-index: -1;
    background-image: url('https://images.unsplash.com/photo-1457364887197-9150188c107b?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1350&q=80');
    background-repeat: no-repeat;
    background-size: cover;
    background-position: 80% 0%;

    &::after {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      z-index: 1;
      width: 100%;
      height: 100vh;
      background: rgba(0,0,0,.2);
    }
  }
</style>

