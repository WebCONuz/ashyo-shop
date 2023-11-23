<script setup lang="ts">
import { ref } from "vue";
import Title from "../ui/element/Title.vue";
import { Swiper, SwiperSlide } from "swiper/vue";
import { Navigation } from "swiper/modules";
import "swiper/css";
import "swiper/css/navigation";

const props = defineProps({
  title: String,
});

const modules = ref<any[]>([Navigation]);
const products: number[] = [1, 2, 3, 4, 5, 6, 7, 8];
</script>

<template>
  <section class="product_slider overflow-x-hidden w-full pb-20">
    <Title>{{ props.title }}</Title>
    <div class="w-[120vw]">
      <swiper
        :slidesPerView="6"
        :spaceBetween="25"
        :pagination="{
          clickable: true,
        }"
        :loop="true"
        :centeredSlides="true"
        :modules="modules"
        class="mySwiper"
      >
        <swiper-slide
          v-for="(item, index) in products"
          :key="index + '-caroucel-item'"
        >
          <div class="slide_item h-[420px] bg-gray-200"></div>
        </swiper-slide>
      </swiper>
    </div>
  </section>
</template>

<style>
.product_slider .swiper-pagination {
  width: auto;
  bottom: 15px;
  top: auto;
  display: flex;
  align-items: center;
}
.product_slider .swiper-pagination .swiper-pagination-bullet {
  background-color: #fff;
  width: 12px;
  height: 12px;
  opacity: 1;
  margin-right: 16px;
}
.product_slider .swiper-pagination .swiper-pagination-bullet-active {
  background-color: #95bef3;
  width: 20px;
  height: 20px;
}
</style>
