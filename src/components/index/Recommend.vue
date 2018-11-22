<template>
    <div>
        <div class="recommend-title">
            <img class="love" src="http://img1.qunarzz.com/piao/fusion/1711/89/ebc329f16c55bb02.png" alt="">
            <span>猜你喜欢</span>    
        </div>
        
        <ul>
           <li class="item" v-for="v in groupList" :key="v.id">
                 <img class="item-img" :src="v.img" alt="">
             <div class="item-info">
                 <p class="item-title">{{v.title}}</p>
                 <p class="item-commentary">
                    <span style="color: #ffb436" class="iconfont">&#xe602;</span>
                    <span class="item-comment">{{v.comment}}条评论</span>
                 </p>
                 <div class="like-price">
                      <p class="item-price">¥<span class="price">{{v.price}}</span></p>起
                      <p class="item-city">{{v.area}}</p>
                 </div>
                 
             </div>
           </li>
      </ul>
    </div>
</template>
<script>
export default {
    name: 'HomeRecommend',
    data () {
        return {
            groupList: [{
                id: '0001',
                img: 'http://img1.qunarzz.com/sight/p0/201404/23/04b92c99462687fa1ba45c1b5ba4ad77.jpg_200x200_4ab5da75.jpg',
                title: '大连圣亚海洋世界',
                comment: 33823,
                price: 99,
                area: '沙河口区'
            },{
                id: '0002',
                img: 'http://img1.qunarzz.com/sight/p0/1707/57/5729585581b6732fa3.water.jpg_200x200_85298361.jpg',
                title: '大连森林动物园',
                comment: 20725,
                price: 48,
                area: '西岗区'
            },{
                id: '0003',
                img: 'http://img1.qunarzz.com/sight/p0/1712/e0/e04c331341c935afa3.water.jpg_200x200_5e3c94ce.jpg',
                title: '东方威尼斯水城',
                comment: 429,
                price: 108,
                area: '大连'
            },{
                id: '0004',
                img: 'http://img1.qunarzz.com/sight/p0/1602/39/39f6b1003abe1b2790.img.jpg_200x200_a7051b04.jpg',
                title: '老虎滩海洋公园',
                comment: 22529,
                price: 50,
                area: '中山区'
            },{
                id: '0005',
                img: 'http://img1.qunarzz.com/sight/p0/1512/f2/f2b803bcf9a4a6a990.water.jpg_200x200_188907c7.jpg',
                title: '大连铭湖国际温泉滑雪度假区',
                comment: 157,
                price: 109,
                area: '瓦房店市'
            },{
                id: '0006',
                img: 'http://img1.qunarzz.com/sight/p0/201309/29/a44c5bc117172352c8d65eac.jpg_200x200_a9c9b119.jpg',
                title: '旅顺开世温泉',
                comment: 420,
                price: 881,
                area: '旅顺口区'
            },{
                id: '0007',
                img: 'http://img1.qunarzz.com/sight/p0/201307/24/1b28192003214460c8d65eac.jpg_200x200_bc6339cb.jpg',
                title: '安波鸿缘温泉山庄',
                comment: 107,
                price: 96,
                area: '普兰店市'
            }]
        }
    }
}
</script>
<style lang="stylus" scoped>
 @import '../../assets/mixins.stl'
.recommend-title 
    margin-top: .2rem
    line-height: .8rem
    background: #eee
    text-indent: .2rem
    font-size: .32rem
    color: #212121
   .love 
        padding-right: .1rem
        width: .3rem
        height: .3rem
        vertical-align: middle
.item 
    display: flex
    height: 2.8rem
    margin: 0 0.24rem
    font-size: .28rem
   .item-img 
      width: 2.1rem
      height: 2.1rem
      padding-top: .3rem
     .item-title 
        font-size: .32rem
     span
        width: .34rem
   .item-info 
       flex: 1    
       padding: .1rem
       margin-left: .12rem
      .item-title 
          line-height: .44rem
          font-size: .37rem
          margin-top: .42rem
          color: #212121
          height: .44rem
          ellipsis()
      .item-commentary
         line-height: .34rem
         font-size: .28rem
         color: #616161
         margin-top: .22rem
         .item-comment 
             margin-left: .30rem
      .like-price 
         position: relative
         width: 100%
         margin-top: .20rem
         font-size: .35rem
         color: #616161
         
        .item-price 
           color: #ff8300
           display: inline-block
          .price
             font-size: .5rem
             color: #ff8300
        .item-city
            position: absolute
            bottom: 0
            right: .24rem
</style>