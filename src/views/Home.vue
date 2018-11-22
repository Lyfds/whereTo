<template>
  <div>
   <home-header></home-header>
   <home-swiper></home-swiper>
   <home-icons></home-icons>
   <home-recommend></home-recommend>
   <home-weekend></home-weekend>
  </div>
</template>

<script>
// @ is an alias to /src
import HomeHeader from '@/components/index/Header.vue'
import HomeSwiper from '@/components/index/Swiper.vue'
import HomeIcons from '@/components/index/Icons.vue'
import HomeRecommend from '@/components/index/Recommend.vue'
import HomeWeekend from '@/components/index/Weekend.vue'

export default {
  name: 'home',
  components: {
    HomeHeader,
    HomeSwiper,
    HomeIcons,
    HomeRecommend,
    HomeWeekend
  },
}
</script>
