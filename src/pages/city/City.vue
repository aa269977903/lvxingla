<template>
  <div>
    <city-header></city-header>
    <city-search></city-search>
    <city-list></city-list>
    我是城市选择
  </div>
</template>

<script>
import CityHeader from './components/Header'
import CitySearch from './components/Search'
import CityList from './components/List'

export default {
  name: 'City',
  components: {
    CityHeader,
    CitySearch,
    CityList
  }
}
</script>

<style scoped>

</style>
