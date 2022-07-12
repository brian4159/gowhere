<template>
  <div class="wrapper">
    <swiper :options="swiperOption"  >
     <swiper-slide v-for="item of swiperList" :key="item.id">
        <img class="swiper-img" 
        :src="item.imgUrl" 
        />
      </swiper-slide>
      
  
    <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
    name:'HomeSwiper',
    data(){
        return{
            swiperOption: {
              pagination:'.swiper-pagination',
              loop:true
        },
        swiperList:[
          {
          id:'0001',
          imgUrl:"https://img1.qunarzz.com/travel/poi/1504/60/1d8518f48e5283.jpg_r_640x290x70_29c73fbf.jpg"
        },
        {id:'0002',
          imgUrl:"https://img1.qunarzz.com/travel/poi/1504/48/43366084ff7fe1.jpg_r_640x290x70_697366f0.jpg" 
          }]
        }
    },
    computed: {
     
    },
  
}
</script>


<style lang="stylus" scoped>
  .wrapper >>> .swiper-pagination-bullet-active
    background: #fff
  .wrapper
    overflow: hidden
    width: 100%
    height: 0
    padding-bottom: 53.4%
    background: #eee
    .swiper-img
      width: 100%
</style>