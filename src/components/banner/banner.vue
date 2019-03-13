<template>
    <mt-swipe :auto="time">
      <mt-swipe-item v-for = "(item, key) in banner" v-show = "item['position'] *1 == 10" :key="key">
        <a :href="item.url ? item.url : 'javascript:;'">
          <img :src="item.photo" :alt="item.title">
        </a>
      </mt-swipe-item>
    </mt-swipe>
</template>

<script>
export default {
  props: {
    time: {
      default: 3000,
      type: Number
    },
    banner: {
      defautl: () => new Array()
    }
  }
}
</script>

<style>
  .mint-swipe .mint-swipe-indicators .mint-swipe-indicator {
    bottom: .23rem;
    opacity: 1;
    background: #fff;
  }
  .mint-swipe .mint-swipe-indicators .is-active  {
    background: #e10030;
  }
</style>
