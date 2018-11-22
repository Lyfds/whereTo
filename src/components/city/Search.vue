<template>
     <div class="search">
        <input class="search-input" type="text" placeholder="输入城市名或拼音" />
     </div>
        
</template>
<script>
export default {
    name: 'CitySearch'
}
</script>
<style lang="stylus" scoped>
@import '../../assets/varibles.stl'
.search
    height: .72rem
    background: $bgColor
    padding: 0 .1rem
    overflow hidden
   .search-input
        width: 100%
        height: .62rem
        box-sizing: border-box
        padding: 0 .2rem
        color: #666
        border-radius: .1rem
        line-height: .62rem
        text-align: center
        float: left
</style>