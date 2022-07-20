<!-- eslint-disable vue/no-multiple-template-root -->
<template>
<div>
  <city-header></city-header>
  <city-search></city-search>
  <city-list></city-list>
</div>
</template>

<script>

// eslint-disable-next-line no-unused-vars
import CityHeader from './components/Header.vue'
import CitySearch from './components/Search.vue'
import CityList from './components/List.vue'
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name:'City',
    components:{
        CityHeader,
        CitySearch,
        CityList
    }
}
</script>

<style>

</style>