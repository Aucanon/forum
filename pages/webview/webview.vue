<template>
  <view>
    <web-view :src=url></web-view>
  </view>
</template>

<script>
  export default {
    data() {
      return {
        url: ''
      };
    },
    onLoad(options) {
      this.url = decodeURI(options.url)
    }
  }
</script>

<style lang="scss">

</style>
