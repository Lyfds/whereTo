<template>
   <div>
       <city-header></city-header>
       <city-search></city-search>
       <city-list></city-list>
   </div>
    
</template>
<script>
import CityHeader from '@/components/city/Header.vue'
import CitySearch from '@/components/city/Search.vue'
import CityList from '@/components/city/List.vue'

export default {
    name: 'City',
    components: {
        CityHeader,
        CitySearch,
        CityList,
    }

}
</script>