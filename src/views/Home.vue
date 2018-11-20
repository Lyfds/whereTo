<template>
  <div>
   <home-header>Hello world</home-header>
  </div>
</template>

<script>
// @ is an alias to /src
import HomeHeader from '@/components/Header.vue'

export default {
  name: 'home',
  components: {
    HomeHeader
  }
}
</script>
