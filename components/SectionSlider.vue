<template>
  <v-lazy
    :min-height="200"
    :options="{ threshold: 0.5 }"
    transition="fade-transition"
  >
    <v-banner data-aos="fade-out" data-aos-duration="1100">
      <v-row id="rowcon">
        <v-col id="txt" cols="12" style="">
          <h2>discover populer orders</h2>
          <p class="subtitle-2">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Non
          </p>
        </v-col>
        <br />
        <v-row>
          <swiper
            :centeredSlides="true"
            :autoplay="{
              delay: 2500,
              disableOnInteraction: false,
            }"
            :scrollbar="{
              hide: true,
            }"
            :pagination="{
              clickable: true,
            }"
            :navigation="true"
            :mousewheel="true"
            :keyboard="true"
            :slides-per-view="3"
            :spaceBetween="30"
            :loop="true"
            :modules="modules"
            class="mySwiper"
            prev-icon="mdi-chevron-left"
            next-icon="mdi-chevron-right"
          >
            <swiper-slide id="swip">
              <img src="/public/img/product-1.png" />

              <h4>marshmalow</h4>
            </swiper-slide>
            <swiper-slide id="swip">
              <img src="/public/img/product-2.png" />

              <h4>Chicogo</h4>
            </swiper-slide>
            <swiper-slide id="swip">
              <img src="/public/img/product-3.png" />

              <h4>New York</h4>
            </swiper-slide>
            <swiper-slide id="swip">
              <img src="/public/img/product-4.png" />

              <h4>Sicilian</h4>
            </swiper-slide>
          </swiper>
        </v-row>
      </v-row>
    </v-banner>
  </v-lazy>
</template>

<script>
import { Swiper, SwiperSlide } from "swiper/vue";
// Import Swiper styles
import "swiper/css";
import "swiper/css/scrollbar";
// import required modules
import { Scrollbar } from "swiper/modules";
// import required modules
import { Autoplay, Navigation, Mousewheel, Keyboard } from "swiper/modules";
export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      products: [
        {
          img: "product-1.png",
          dis: "marshmalow",
        },
        {
          img: "/public/img/product-2.png",
          dis: "meet",
        },
        {
          img: "/public/img/product-3.png",
          dis: "mogzrilla",
        },
        {
          img: "/public/img/product-4.png",
          dis: "furuts",
        },
      ],
      dispro: "",
    };
  },
  setup() {
    return {
      modules: [Navigation, Mousewheel, Keyboard, Scrollbar, Autoplay],
    };
  },
};
</script>

<style scoped>
#txt {
  text-align: center;
}
#swip img {
  width: 200px;
}
/*/tablet/*/
@media (max-width: 991px) {
  #swip img {
    width: 180px;
  }
}
/*/mobile/*/
@media (max-width: 500px) {
  #txt {
    left: -70px;
    position: relative;
  }
  #rowcon {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .mySwiper {
    width: 70%;
    height: 200px;
    position: relative;
    left: -70px;

    background-image: url(/public/img/popular-dish.png);
    background-position-x: center;
    background-repeat: no-repeat;
    background-size: 150px;
  }
  #swip {
    display: flex;
    flex-flow: column;
    justify-content: center;
    align-items: center;
  }
}
#rowcon {
  display: flex;
  justify-content: center;
  align-items: center;
}
.mySwiper {
  width: 70%;
  height: 200px;
  padding: 5px;
  position: relative;


  background-image: url(/public/img/popular-dish.png);
  background-position-x: center;
  background-repeat: no-repeat;
  background-size: 150px;
}
#swip {
  display: flex;
  flex-flow: column;
  justify-content: center;
  align-items: center;
}
h4 {
  display: none;
}
div#swip.swiper-slide-active h4 {
  display: flex;
  transition: all, 2s;
  scale: 1.2;
  margin-top: 20px;
}
div#swip.swiper-slide-active img {
  display: flex;
  transition: all, 2s;
  scale: 1.1;
  transform: rotateZ(-80deg);
  perspective: 200px;
}
#swip img {
  height: 120px;
  width: 120px;
}
</style>
