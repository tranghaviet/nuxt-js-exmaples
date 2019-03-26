<template>
  <div>
    <swiper ref="mySwiper" :options="swiperOption">
      <!-- slides -->
      <swiper-slide>
        <img
          src="http://static.asiawebdirect.com/m/bangkok/portals/vietnam/homepage/hanoi/pagePropertiesOgImage/teaser_006.jpg.jpg">
      </swiper-slide>
      <swiper-slide>
        <img
          src="http://static.asiawebdirect.com/m/bangkok/portals/vietnam/homepage/hanoi/pagePropertiesOgImage/teaser_006.jpg.jpg">
      </swiper-slide>
      <swiper-slide>
        <img
          src="http://static.asiawebdirect.com/m/bangkok/portals/vietnam/homepage/hanoi/pagePropertiesOgImage/teaser_006.jpg.jpg">
      </swiper-slide>
      <swiper-slide>
        <img
          src="http://static.asiawebdirect.com/m/bangkok/portals/vietnam/homepage/hanoi/pagePropertiesOgImage/teaser_006.jpg.jpg">
      </swiper-slide>
      <!-- Optional controls -->
      <div slot="pagination" class="swiper-pagination" />
      <div slot="button-prev" class="swiper-button-prev" />
      <div slot="button-next" class="swiper-button-next" />
      <!--<div slot="scrollbar" class="swiper-scrollbar" />-->
    </swiper>
  </div>
</template>

<script>
import { swiper, swiperSlide } from 'vue-awesome-swiper'

export default {
  name: 'SwiperCarousel',
  components: {
    swiper,
    swiperSlide
  },
  data() {
    return {
      swiperOption: {
        slidesPerView: 2,
        spaceBetween: 30,
        navigation: {
          nextEl: '.swiper-button-next',
          prevEl: '.swiper-button-prev',
        },
      }
    }
  },
}
</script>

<style lang="scss">
  .swiper-slide {
    img {
      max-width: 100%;
    }
  }
</style>
