<template>
    <div class="navbar">
      <div class="left">
        <slot name="left"></slot>
      </div>
      <div class="center">
        <slot name="center"></slot>
      </div>
      <div class="right">
        <slot name="right"></slot>
      </div>
    </div>
</template>

<script>
  export default {
    name: 'NavBar',
    data() {
      return {
        
      }
    }
  }
</script>

<style>
  .navbar{
    display: flex;
    height: 44px;
    line-height: 44px;
    text-align: center;
    box-shadow: 0 1px 1px rgba(100, 100, 100, .1);
  }
   .left, .right{
    width: 44px;
    height: 44px;
  }
  .center{
    flex: 1;
  }
</style>