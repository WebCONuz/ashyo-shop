<script setup lang="ts"></script>

<template>
  <section class="logo-grid">
    <div class="container pt-5 pb-[100px] bg-white">
      <div class="grid grid-container">
        <router-link
          to="#"
          class="item1 bg-[#5C4F8C] rounded-md flex items-center justify-center text-white relative"
        >
          <button
            class="outline-none border border-white bg-transparent py-1 px-3 rounded-[20px] absolute top-5 left-5 z-10"
          >
            Noutbooklar
          </button>
          <img
            src="../../assets/images/category/laptop.png"
            alt="laptop"
            class="absolute bottom-0 right-6"
          />
        </router-link>
        <router-link
          to="#"
          class="item2 bg-[#A09188] rounded-md flex items-center justify-center text-white relative"
        >
          <button
            class="outline-none border border-white bg-transparent py-1 px-3 rounded-[20px] absolute top-5 left-5 z-10"
          >
            Kiryuvish mashinasi
          </button>
          <img
            src="../../assets/images/category/wash.png"
            alt="wash machine"
            class="absolute bottom-0 right-0"
          />
        </router-link>
        <router-link
          to="#"
          class="item3 bg-[#797C7D] rounded-md flex items-center justify-center text-white relative"
        >
          <button
            class="outline-none border border-white bg-transparent py-1 px-3 rounded-[20px] absolute top-5 left-5 z-10"
          >
            Kondetsiyoner
          </button>
          <img
            src="../../assets/images/category/contitsioner.png"
            alt="contitsioner"
            class="absolute top-11 right-0"
          />
        </router-link>
        <router-link
          to="#"
          class="item4 bg-[#CEAF75] rounded-md flex items-center justify-center text-white relative"
        >
          <button
            class="outline-none border border-white bg-transparent py-1 px-3 rounded-[20px] absolute top-5 left-5 z-10"
          >
            Televizorlar
          </button>
          <img
            src="../../assets/images/category/tv.png"
            alt="tv"
            class="h-full absolute bottom-0 right-7"
          />
        </router-link>
        <router-link
          to="#"
          class="item5 bg-[#676D86] rounded-md flex items-center justify-center text-white relative"
        >
          <button
            class="outline-none border border-white bg-transparent py-1 px-3 rounded-[20px] absolute top-5 left-5 z-10"
          >
            Smartfonlar
          </button>
          <img
            src="../../assets/images/category/phone.png"
            alt="phone"
            class="h-full absolute bottom-0 right-0"
          />
        </router-link>
        <router-link
          to="#"
          class="item6 bg-[#888380] rounded-md flex items-center justify-center text-white relative"
        >
          <button
            class="outline-none border border-white bg-transparent py-1 px-3 rounded-[20px] absolute top-5 left-5"
          >
            Muzlatgichlar
          </button>
          <div
            class="absolute top-0 right-0 z-10 h-full w-8 bg-[#888380] translate-x-1/2"
          ></div>
          <img
            src="../../assets/images/category/fridge1.png"
            alt="fridge-1"
            class="w-[118px] absolute bottom-0 right-0 z-20 translate-x-[70%]"
          />
        </router-link>
        <router-link
          to="#"
          class="item7 bg-[#888380] rounded-md flex items-center justify-center text-white relative"
        >
          <img
            src="../../assets/images/category/frigde2.png"
            alt="fridge-2"
            class="absolute bottom-0 right-0 z-10"
          />
        </router-link>
        <router-link
          to="#"
          class="item8 bg-[#134E9B] rounded-md flex items-center justify-center text-white"
          >Ko’proq</router-link
        >
      </div>
    </div>
  </section>
</template>

<style scoped>
.grid-container {
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
  grid-template-rows: 58px 58px 58px 58px 58px 58px 58px 58px;
  grid-gap: 10px;
}
.grid-container .item1 {
  grid-column: 1/3;
  grid-row: 1/5;
}
.grid-container .item2 {
  grid-column: 1/2;
  grid-row: 5/9;
}
.grid-container .item3 {
  grid-column: 3/4;
  grid-row: 1/5;
}
.grid-container .item4 {
  grid-column: 2/4;
  grid-row: 5/9;
}
.grid-container .item5 {
  grid-column: 4/5;
  grid-row: 1/5;
}
.grid-container .item6 {
  grid-column: 4/5;
  grid-row: 5/9;
}
.grid-container .item7 {
  grid-column: 5/6;
  grid-row: 2/9;
}
.grid-container .item8 {
  grid-column: 5/6;
  grid-row: 1/2;
}
</style>
