<!-- eslint-disable vue/no-multiple-template-root -->

<template>
   <div>
   <home-header></home-header>
    <home-swiper></home-swiper>
    <home-icons></home-icons>
   </div>
    
</template>

<script>
import HomeHeader from './components/Header'
import HomeSwiper from './components/Swiper'
import HomeIcons from './components/Icons'
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name:'Home',
    components:{
     
        HomeHeader,
        // eslint-disable-next-line vue/no-unused-components
        HomeSwiper,
        // eslint-disable-next-line vue/no-unused-components
        HomeIcons
        
    }
}
</script>

<style>

</style>