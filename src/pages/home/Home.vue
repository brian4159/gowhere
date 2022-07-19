<!-- eslint-disable vue/no-multiple-template-root -->

<template>
   <div>
   <home-header></home-header>
    <home-swiper></home-swiper>
    <home-icons></home-icons>
    <home-recommend></home-recommend>
    <home-weekend></home-weekend>
   </div>
    
</template>

<script>
import HomeHeader from './components/Header'
import HomeSwiper from './components/Swiper'
import HomeIcons from './components/Icons'
import HomeRecommend from './components/Recommend'
import HomeWeekend from './components/Weekend'
import axios from 'axios'
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name:'Home',
    components:{
     
        HomeHeader,
        // eslint-disable-next-line vue/no-unused-components
        HomeSwiper,
        // eslint-disable-next-line vue/no-unused-components
        HomeIcons,
        // eslint-disable-next-line vue/no-unused-components
        HomeRecommend,
        HomeWeekend
        
    },
    methods:{
        getHomeInfo(){
            axios.get('')
            .then(this.getHomeInfoSucc)
        },
        getHomeInfoSucc(res){
            console.log(res);
        }
    },
    mounted (){
        this.getHomeInfo()
    }
}
</script>

<style>

</style>