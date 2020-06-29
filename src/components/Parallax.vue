<template>
  <div class="parallax">
  </div>    
</template>

<script>
export default {
  name: 'Parallax',
  props: {
   
  }
}
</script>

<style scoped lang="stylus">
  div.parallax
    width 100%
    height 10rem
    background-image url(../assets/forest1.jpg)
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
</style>
