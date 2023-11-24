<script setup lang="ts">
import ProductCard from "../components/ui/card/ProductCard.vue";
</script>

<template>
  <main class="product">
    <div class="container flex text-[#B6BABF] text-sm">
      Bosh sahifa / Smartfonlar /
    </div>
    <div class="container mt-6 flex items-start">
      <aside
        class="min-h-screen w-1/4 bg-[#EBEFF3] overflow-y-auto py-[18px] px-[19px] rounded-lg"
      >
        <div class="flex items-end mb-4">
          <span class="font-medium mr-2">Narx</span>
          <span class="text-sm">[so‘m]</span>
        </div>
        <div class="flex mb-[26px] gap-x-1">
          <div class="w-1/2">
            <span class="text-gray-400">..dan</span>
            <div
              class="bg-white py-2 text-center rounded-[5px] text-sm leading-[34px] text-gray-600 mt-[6px]"
            >
              2 000 000
            </div>
          </div>
          <div class="w-1/2">
            <span class="text-gray-400">..gacha</span>
            <div
              class="bg-white py-2 text-center rounded-[5px] text-sm leading-[34px] text-gray-600 mt-[6px]"
            >
              20 000 000
            </div>
          </div>
        </div>
      </aside>
      <div class="w-3/4 min-h-screen flex flex-wrap">
        <div class="card_wrapper"><ProductCard /></div>
        <div class="card_wrapper"><ProductCard /></div>
        <div class="card_wrapper"><ProductCard /></div>
        <div class="card_wrapper"><ProductCard /></div>
        <div class="card_wrapper"><ProductCard /></div>
        <div class="card_wrapper"><ProductCard /></div>
        <div class="card_wrapper"><ProductCard /></div>
        <div class="card_wrapper"><ProductCard /></div>
        <div class="card_wrapper"><ProductCard /></div>
      </div>
    </div>
  </main>
</template>

<style scoped>
.card_wrapper {
  width: calc(100% / 3 - 20px);
  margin: 0 0 40px 20px;
}
</style>
