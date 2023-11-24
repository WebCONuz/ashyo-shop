<script setup lang="ts"></script>

<template>
  <section class="logo-grid">
    <div class="container py-[100px] bg-white">
      <div class="grid grid-container">
        <div
          class="item item1 flex items-center justify-center bg-[#E1F0D7] rounded-md overflow-hidden"
        >
          <img
            src="../../assets/images/company/artel.png"
            alt="logo"
            class="duration-200"
          />
        </div>
        <div
          class="item item2 flex items-center justify-center bg-[#E6E6E6] rounded-md overflow-hidden"
        >
          <img
            src="../../assets/images/company/apple.png"
            alt="logo"
            class="duration-200"
          />
        </div>
        <div
          class="item item3 flex items-center justify-center bg-[#E6EEF6] rounded-md overflow-hidden"
        >
          <img
            src="../../assets/images/company/samsung.png"
            alt="logo"
            class="duration-200"
          />
        </div>
        <div
          class="item item4 flex items-center justify-center bg-[#CCE2F1] rounded-md overflow-hidden"
        >
          <img
            src="../../assets/images/company/vivo.png"
            alt="logo"
            class="duration-200"
          />
        </div>
        <div
          class="item item5 flex items-center justify-center bg-[#E0E8F3] rounded-md overflow-hidden"
        >
          <img
            src="../../assets/images/company/nokia.png"
            alt="logo"
            class="duration-200"
          />
        </div>
        <div
          class="item item6 flex items-center justify-center bg-[#FFD1D2] rounded-md overflow-hidden"
        >
          <img
            src="../../assets/images/company/huawei.png"
            alt="logo"
            class="duration-200"
          />
        </div>
        <div
          class="item item7 flex items-center justify-center bg-[#FFE1CC] rounded-md overflow-hidden"
        >
          <img
            src="../../assets/images/company/mi.png"
            alt="logo"
            class="duration-200"
          />
        </div>
        <div class="item item8 bg-[#EBEFF3] rounded-md">
          <router-link
            to="#"
            class="w-full h-full flex items-center justify-center text-[#134E9B] font-medium"
          >
            Ko’proq
          </router-link>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.grid-container {
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-template-rows: 45px 45px 45px 45px 45px 45px;
  grid-gap: 10px;
}
.grid-container .item:hover img {
  transform: scale(1.1);
}
.grid-container .item1 {
  grid-column: 1/2;
  grid-row: 1/3;
}
.grid-container .item2 {
  grid-column: 1/2;
  grid-row: 3/7;
}
.grid-container .item3 {
  grid-column: 2/3;
  grid-row: 1/5;
}
.grid-container .item4 {
  grid-column: 2/3;
  grid-row: 5/7;
}
.grid-container .item5 {
  grid-column: 3/4;
  grid-row: 1/4;
}
.grid-container .item6 {
  grid-column: 3/4;
  grid-row: 4/7;
}
.grid-container .item7 {
  grid-column: 4/5;
  grid-row: 1/6;
}
.grid-container .item8 {
  grid-column: 4/5;
  grid-row: 6/7;
}
</style>
