<template>
    <div class="header">
          城市选择
        <router-link to="/">
        <div class="iconfont header-icon">&#xe624;</div>
        </router-link>
    </div>
</template>
<script>
export default {
    name: 'CityHeader'
}
</script>
<style lang="stylus" scoped>
@import '../../assets/varibles.stl'
.header 
    position: relative
    font-size: .40rem
    overflow: hidden
    height: .86rem
    line-height: .86rem
    text-align: center
    color: #fff
    background: $bgColor
   .header-icon 
       position: absolute
       left: 0
       top: 0
       width: .86rem
       text-align: center
       font-size: .4rem
       color: #fff

</style>
