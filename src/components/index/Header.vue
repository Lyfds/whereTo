<template>
  <div class="header">
     <div class="header-left">
        <div class="iconfont back-icon">&#xe624;</div>
     </div>
     <div class="header-input">
        <span class="iconfont">&#xe632;</span>
       输入游玩城市/景点/游玩主题</div>
      <router-link to="/city">
     <div class="header-right">
       城市
       <span class="iconfont arrow-icon">&#xe600;</span>
      </div>
      </router-link>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader',

}
</script>
<style lang="stylus" scoped>
  @import '../../assets/varibles.stl'
 .header 
      display: flex
      line-height: .82rem
      background: $bgColor
      color: #fff
      font-size: .32rem
    .header-left 
        float: left
        width: .84rem
        .back-icon 
            text-align: center
            font-size: .4rem
    .header-input 
        flex:1
        line-height: .62rem
        background: #fff
        border-radius:.1rem 
        margin-top: .12rem
        height: .62rem
        margin-left: .2rem
        padding-left: .2rem
        color: #ccc
    .header-right
        float: right
        width: 1.24rem
        color: #fff
        text-align: center
        .arrow-icon 
           font-size: .2rem
           margin-left: -.04rem
</style>

