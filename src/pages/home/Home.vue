<!-- eslint-disable vue/no-multiple-template-root -->

<template>
   <div>
   <home-header></home-header>
    <home-swiper></home-swiper>
    <div>test</div>
   </div>
    
</template>

<script>
import HomeHeader from './components/Header'
import HomeSwiper from './components/Swiper'
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name:'Home',
    components:{
     
        HomeHeader,
        // eslint-disable-next-line vue/no-unused-components
        HomeSwiper
        
    }
}
</script>

<style>

</style>