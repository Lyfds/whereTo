<template>
    <div>
        <div class="recommend-title">
            <span>周末去哪儿</span>    
        </div> 
        <div class="produce-item" v-for="v in groupList" :key="v.id">
            <div class="product-imgcontainer">
                 <img :src="v.img" alt="">
            </div>
            <div class="product-info">
                   <p class="product-name">{{v.name}}</p>
                   <p class="product-desc">{{v.desc}}</p>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'HomeWeekend',
    data () {
        return {
            groupList: [{
                id: '0001',
                img: 'http://img1.qunarzz.com/sight/source/1505/9f/f585152825459.jpg_r_640x214_5d46e4cc.jpg',
                name: '温泉水上乐园',
                desc: '泡泡温泉，吹吹海风，深觉人生美好'
            },{
               id: '0002',
                img: 'http://img1.qunarzz.com/sight/source/1505/9f/f585152825459.jpg_r_640x214_5d46e4cc.jpg',
                name: '温泉水上乐园',
                desc: '泡泡温泉，吹吹海风，深觉人生美好'
            },{
               id: '0003',
                img: 'http://img1.qunarzz.com/sight/source/1505/9f/f585152825459.jpg_r_640x214_5d46e4cc.jpg',
                name: '温泉水上乐园',
                desc: '泡泡温泉，吹吹海风，深觉人生美好'
            },{
               id: '0004',
                img: 'http://img1.qunarzz.com/sight/source/1505/9f/f585152825459.jpg_r_640x214_5d46e4cc.jpg',
                name: '温泉水上乐园',
                desc: '泡泡温泉，吹吹海风，深觉人生美好'
            },{
              id: '0005',
                img: 'http://img1.qunarzz.com/sight/source/1505/9f/f585152825459.jpg_r_640x214_5d46e4cc.jpg',
                name: '温泉水上乐园',
                desc: '泡泡温泉，吹吹海风，深觉人生美好'
            },{
               id: '0006',
                img: 'http://img1.qunarzz.com/sight/source/1505/9f/f585152825459.jpg_r_640x214_5d46e4cc.jpg',
                name: '温泉水上乐园',
                desc: '泡泡温泉，吹吹海风，深觉人生美好'
            },{
               id: '0007',
                img: 'http://img1.qunarzz.com/sight/source/1505/9f/f585152825459.jpg_r_640x214_5d46e4cc.jpg',
                name: '温泉水上乐园',
                desc: '泡泡温泉，吹吹海风，深觉人生美好'
            }]
        }
    }
}
</script>
<style lang="stylus" scoped>
 @import '../assets/mixins.stl'
.recommend-title 
    margin-top: .2rem
    line-height: .8rem
    background: #eee
    text-indent: .2rem
    font-size: 16px
    color: #212121
.product-item
    height: 2.04rem
   .product-imgcontainer
        overflow: hidden
        height: 0
        padding-bottom: 35%
        img 
           opacity: 1
    .product-info
       font-size: .22rem
       color: #616161
       line-height: .42rem
       padding: .15rem .3rem .3rem .2rem
      .product-name
            color: #212121;
            font-size: .3rem;
            ellipsis()
      .product-desc
           ellipsis()

</style>