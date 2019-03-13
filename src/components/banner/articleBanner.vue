<template>
  <div class="bannerBox" v-if="adPass ? adPass.length > 0 : adPass">
    <swiper :options="swiperOption">
      <swiper-slide v-for="(item, key) in adPass" :key="key">
        <a :href="item.url"><img style="width: 3.45rem; height: 2.14rem;" :src="item.photo" alt=""></a>
      </swiper-slide>
    </swiper>
  </div>
</template>

<script type='text/ecmascript-6'>
export default {

}
</script>

<style scoped lang='less'>
  .bannerBox {
    height: 2.14rem;
    width: 7.1rem;
    margin: 0 auto;
    padding-top: .3rem;
    position: relative;
    overflow: hidden;
    img {
      height: 100%;
      width: 100%;
    }
  }
</style>
