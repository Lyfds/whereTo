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
                img: 'http://img1.qunarzz.com/sight/p0/201404/23/04b92c99462687fa1ba45c1b5ba4ad77.jpg_200x200_4ab5da75.jpg',
                title: '大连圣亚海洋世界',
                comment: 33823,
                price: 99,
                area: '沙河口区'
            },{
                id: '0003',
                img: 'http://img1.qunarzz.com/sight/p0/201404/23/04b92c99462687fa1ba45c1b5ba4ad77.jpg_200x200_4ab5da75.jpg',
                title: '大连圣亚海洋世界',
                comment: 33823,
                price: 99,
                area: '沙河口区'
            },{
                id: '0004',
                img: 'http://img1.qunarzz.com/sight/p0/201404/23/04b92c99462687fa1ba45c1b5ba4ad77.jpg_200x200_4ab5da75.jpg',
                title: '大连圣亚海洋世界',
                comment: 33823,
                price: 99,
                area: '沙河口区'
            },{
                id: '0005',
                img: 'http://img1.qunarzz.com/sight/p0/201404/23/04b92c99462687fa1ba45c1b5ba4ad77.jpg_200x200_4ab5da75.jpg',
                title: '大连圣亚海洋世界',
                comment: 33823,
                price: 99,
                area: '沙河口区'
            },{
                id: '0006',
                img: 'http://img1.qunarzz.com/sight/p0/201404/23/04b92c99462687fa1ba45c1b5ba4ad77.jpg_200x200_4ab5da75.jpg',
                title: '大连圣亚海洋世界',
                comment: 33823,
                price: 99,
                area: '沙河口区'
            },{
                id: '0007',
                img: 'http://img1.qunarzz.com/sight/p0/201404/23/04b92c99462687fa1ba45c1b5ba4ad77.jpg_200x200_4ab5da75.jpg',
                title: '大连圣亚海洋世界',
                comment: 33823,
                price: 99,
                area: '沙河口区'
            }]
        }
    }
}
</script>
<style lang="stylus" scoped>
.recommend-title 
    margin-top: .2rem
    line-height: .8rem
    background: #eee
    text-indent: .2rem
    font-size: 16px
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
    font-size: 14px
   .item-img 
      width: 2.1rem
      height: 2.1rem
      padding-top: .3rem
     .item-title 
        font-size: 16px  
     span
        width: .34rem
   .item-info 
       flex: 1    
       padding: .1rem
       margin-left: .12rem
      .item-title 
          line-height: .44rem
          font-size: .42rem
          margin-top: .42rem
          color: #212121
          height: .44rem
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