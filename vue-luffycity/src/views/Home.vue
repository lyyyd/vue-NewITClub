<template>
  <el-carousel :interval="5000" arrow="always" height="520px">
    <el-carousel-item v-for="item in imgLinks" :key="item.id">
        <img :src="item.imgSrc" alt="">
    </el-carousel-item>
  </el-carousel>
</template>

<script>

export default {
  name: 'home',
    data(){
      return {
          imgLinks: [
                    {
                        id: 1,
                        imgSrc: "https://hcdn1.luffycity.com/static/frontend/index/banner1(4)_1539945492.0492468.png"
                    },
                    {
                        id: 2,
                        imgSrc: "https://hcdn1.luffycity.com/static/frontend/index/骑士(1)_1539945488.713867.png"
                    },
                    {
                        id: 3,
                        imgSrc: "https://hcdn1.luffycity.com/static/frontend/index/banner11_1538122470.2779157.png"
                    },
                    {
                        id: 4,
                        imgSrc: "https://hcdn1.luffycity.com/static/frontend/index/home-banner4_1535545832.4715614.png"
                    }
                ]
      }
    }
}
</script>

<style scoped>
    img {
        height: 520px;
        width: 100%;
    }
</style>
