<script setup lang="ts">
import { ref } from "vue";
import UIBtn from "../ui/btn/UIBtn.vue";
import { Swiper, SwiperSlide } from "swiper/vue";
import { Autoplay, Pagination } from "swiper/modules";
import "swiper/css";
import "swiper/css/pagination";
import Banner1 from "../../assets/images/banner/banner1.png";
import Banner2 from "../../assets/images/banner/banner2.png";
import Banner3 from "../../assets/images/banner/banner3.png";
import Banner4 from "../../assets/images/banner/banner4.png";
import Banner5 from "../../assets/images/banner/banner5.png";
import Banner6 from "../../assets/images/banner/banner6.png";

const modules = ref<any[]>([Autoplay, Pagination]);
const bg_images: object[] = [
  {
    bgColor: "#F3F0F0",
    color: "#0F4A97",
    url: Banner1,
  },
  {
    bgColor: "rgba(255, 207, 156, 0.2)",
    color: "#EB9F6B",
    url: Banner2,
  },
  {
    bgColor: "rgba(172, 237, 155, 0.4)",
    color: "#71B943",
    url: Banner3,
  },
  {
    bgColor: "rgba(174, 79, 255, 0.2)",
    color: "#6C0DBD",
    url: Banner4,
  },
  {
    bgColor: "rgba(149,201,236, 0.2)",
    color: "#1F91C3",
    url: Banner5,
  },
  {
    bgColor: "#D0D2D5",
    color: "rgb(0,0,0,0.5)",
    url: Banner6,
  },
];
</script>

<template>
  <section class="intro">
    <swiper
      :slidesPerView="1"
      :spaceBetween="25"
      :pagination="{
        clickable: true,
      }"
      :loop="true"
      :centeredSlides="true"
      :autoplay="{
        delay: 4500,
        disableOnInteraction: false,
      }"
      :modules="modules"
      class="mySwiper"
    >
      <swiper-slide
        v-for="(item, index) in bg_images"
        :key="index + '-caroucel-item'"
        :style="`background-color: ${item.bgColor};`"
      >
        <div
          class="container slide_item h-[490px] overflow-hidden flex items-center pt-10"
        >
          <div class="w-1/2">
            <h2
              class="text-[#0A1729] text-[44px] font-black leading-[120%] max-w-[596px] mb-[6px]"
            >
              Siz kutgan Xiaomi 12 Mi Laite
            </h2>
            <p class="max-w-[596px] text-[#545D6A] mb-[22px] text-justify">
              Orginallik va qulay narxni o'zida jamlagan Xiaomi 12 Mi Laite siz
              uchun eng yaxshi arziydigan takliflarimizdan biridir!ii
            </p>
            <UIBtn :style="`background-color: ${item.color};`">
              <p class="text-white w-[129px] py-1">Batafsil</p>
            </UIBtn>
          </div>
          <div class="w-1/2 h-full overflow-hidden relative">
            <img
              :src="item.url"
              alt="banner"
              class="w-[70%] absolute right-0 bottom-0"
            />
          </div>
        </div>
      </swiper-slide>
    </swiper>
  </section>
</template>

<style>
.intro .swiper-pagination {
  width: auto;
  top: auto;
  bottom: 25px;
  left: 6rem;
  right: auto;
  display: flex;
  align-items: center;
  overflow: visible;
}
.intro .swiper-pagination .swiper-pagination-bullet {
  background-color: #fff;
  width: 12px;
  height: 12px;
  opacity: 1;
  margin-right: 16px;
}
.intro .swiper-pagination .swiper-pagination-bullet-active {
  background-color: #95bef3;
  position: relative;
}
.intro .swiper-pagination .swiper-pagination-bullet-active::before {
  content: "";
  width: 100%;
  height: 100%;
  background-color: white;
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
  transform: scale(2.5);
  border-radius: 50%;
}
</style>
