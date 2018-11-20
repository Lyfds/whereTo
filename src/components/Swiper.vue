<template>
  <div class="wrapper">
    <swiper :options="swiperOption" v-if="swiperList.length>1">
    <!-- slides -->
    <swiper-slide v-for="item of swiperList" :key="item.id">
        <img class="swiper-img" :src="item.imgUrl" alt="">
    </swiper-slide>
    <!-- Optional controls -->
    <div class="swiper-pagination" slot="pagination"></div>
  </swiper>
  </div>
</template>
<script>
export default {
    name: 'HomeSwiper',
    data() {
       return {
           swiperOption: {
               pagination: { 
                   el:'.swiper-pagination',   
                   },
                   loop: true
           },
           swiperList: [{
               id:'0001',
               imgUrl: 'http://img1.qunarzz.com/piao/fusion/1811/7c/8e5c4ab8ee8b7402.jpg_750x200_dd7a38dd.jpg',
               
           },{
               id:'0002',
               imgUrl: 'http://img1.qunarzz.com/piao/fusion/1811/4d/6706bf772c05ce02.jpg_750x200_773e75f0.jpg'
           },{
            id:'0003',
            imgUrl: 'http://img1.qunarzz.com/piao/fusion/1811/68/c66e4cde1ee62602.jpg_750x200_e9b97acd.jpg'
           },{
             id:'0004',
             imgUrl:'http://img1.qunarzz.com/piao/fusion/1811/ce/77e115fea8f99102.jpg_750x200_a2d0fcd2.jpg'
           },{
             id:'0005',
             imgUrl: 'http://img1.qunarzz.com/piao/fusion/1810/6e/4a5551bbb189d902.jpg_750x200_25257467.jpg'
           },{
             id:'0006',
             imgUrl: 'http://img1.qunarzz.com/piao/fusion/1811/39/6b1f0402bb1d5902.jpg_750x200_3c7661d6.jpg'
           },{
              id:'0007',
              imgUrl: 'http://img1.qunarzz.com/piao/fusion/1811/4d/b3ce0d8e8cec1802.jpg_750x200_f4a1e0d6.jpg'
           }]
       }
    }
}
</script>
<style lang="stylus" scoped>
.wrapper  >>> .swiper-pagination-bullet-active 
   background : #fff
.wrapper 
   width: 100%
   overflow hidden
   height: 0
   padding-bottom: 26.25%
   background: #ccc
   .swiper-img 
       width: 100%
</style>
