<template>
  <div class="slider">
      <div class="slider-group">
          <slot></slot>
      </div>
      <div class="dots"></div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped lang="stylus">
    @import "common/stylus/variable"
    
    .slider
        min-height 1px
        .slider-group
            position relative
            overflow hidden
            white-space nowrap
</style>
