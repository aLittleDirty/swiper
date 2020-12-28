<template>
  <div class="swiper-container">
    <img class="swiper-image" v-for="(item, index) in imageList" :key="index" :src="item.src"/>
  </div>
</template>
<script>
export default {
  data() {
    return{
      imageList: [{
        src: require('./assets/bg.jpeg')
      },{
        src: require('./assets/bg.jpeg')
      },{
        src: require('./assets/bg.jpeg')
      },{
        src: require('./assets/bg.jpeg')
      },{
        src: require('./assets/bg.jpeg')
      }]
    }
  }
}
</script>
<style scoped>
  .swiper-container {
    border: 1px solid #000000;
    width: 1000px;
    height: 100px;
  }

  .swiper-container .swiper-image {
    width: 200px;
    height: 100px;
  }

</style>