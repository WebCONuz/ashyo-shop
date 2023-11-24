<script setup lang="ts">
import UIBtn from "../btn/UIBtn.vue";
import CartIcon from "../../icons/CartIcon.vue";
import CompareIcon from "../../icons/CompareIcon.vue";
</script>

<template>
  <div class="product-card">
    <router-link
      to="#"
      class="w-full bg-[#EBEFF3] rounded-lg flex items-center justify-center h-[280px] overflow-hidden mb-4"
    >
      <img
        src="../../../assets/images/product.png"
        alt="product-img"
        class="w-[210px]"
      />
    </router-link>
    <h3 class="text-sm text-[#545D6A] mb-7 leading-[19px]">
      Смартфон Xiaomi 12 Lite 8/128Gb Қора kamera 48/68 px
    </h3>
    <p class="text-[#0A1729] text-xl font-bold leading-[26px] mb-[10px]">
      6 999 999 usz
    </p>
    <div class="flex items-end justify-between">
      <router-link
        to="#"
        class="bg-[#FEEAF5] text-[#F02C96] text-sm py-[7px] px-[10px] inline-block rounded-md"
        >6 oy / 1 200 000 usz</router-link
      >
      <UIBtn class="details bg-white px-[14px] border border-[#EBEFF3]">
        <CompareIcon />
      </UIBtn>
      <UIBtn class="cart_btn bg-[#134E9B] px-[14px]">
        <CartIcon />
      </UIBtn>
    </div>
  </div>
</template>

<style>
.cart_btn svg path {
  fill: #fff;
}
</style>
