<template>
  <section :class="cname"> <!--自定义样式cname，因为swiper.css已经写好了默认样式，所以不必写。-->
    <swiper :options="options" :not-next-tick="options.notNextTick"> <!--官方要求使用options来传参-->
      <swiper-slide v-for="item in items" :key="item.href">
        <router-link :to="{ name: item.href}">
          <img :src="item.src" alt="">
        </router-link>
      </swiper-slide>
      <div class="swiper-pagination" v-if="options.pagination"/>
    </swiper>
  </section>
</template>

<script>
import { swiper, swiperSlide } from "vue-awesome-swiper"
export default {
  components: {
    swiper,
    swiperSlider,
  },
  props: {
    options: {
      type: Object,
      default () { //es6写法
        return {
          autoplay: true,//自动轮播
          loop: true,//循环
          pagination: { //指示器
            el: ".swiper-pagination",
          },
          notNextTick: false,
        }
      }
    },
    items: {
      type: Object,
      default () {
        return []
      },
    }
  }
}
</script>

<style lang="css">
  @import "~swiper/dist/css/swiper.css"
</style>