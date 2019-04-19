<template>
  <div class="swiper_content">
    <swiper :options="swiperOption">
      <swiper-slide>
        <div class="coin_content">
          <div class="logo">
            <img src="../assets/logo1.png" alt>
          </div>
        </div>
      </swiper-slide>
      <swiper-slide>Slide 2</swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
import "swiper/dist/css/swiper.css";
import { swiper, swiperSlide } from "vue-awesome-swiper";
export default {
  name: "",
  components: {
    swiper,
    swiperSlide
  },
  data() {
    return {
      swiperOption: {
        direction: "vertical",
        autoplay: true,
        speed: 300,
        pagination: {
          el: ".swiper-pagination",
          clickable: true,
          currentClass: "bullet_current"
        }
      }
    };
  }
};
</script>

<style lang="less" scoped>
.swiper_content {
  width: 1280px;
  margin: 20px auto 0;
  height: 100px;
  .swiper-container {
    height: 100px;
    width: 100%;
    background: rgba(38, 47, 56, 1);
    color: #fff;
    .coin_content {
      display: flex;
      flex-direction: column;
      justify-content: center;
    }
  }
}
</style>