<script setup lang="ts"></script>

<template>
  <footer class="footer pt-5 pb-[69px] bg-white">
    <div class="container flex justify-between">
      <div class="w-1/3">
        <h4 class="text-xl mb-[21px] text-[#4F4F4F] font-bold">
          Bizning ijtimoiy tarmoqlarda
        </h4>
        <div class="flex mb-10">
          <div
            class="w-11 h-10 bg-[#EBEFF3] rounded-md flex items-center justify-center mr-[10px]"
          ></div>
          <div
            class="w-11 h-10 bg-[#EBEFF3] rounded-md flex items-center justify-center mr-[10px]"
          ></div>
          <div
            class="w-11 h-10 bg-[#EBEFF3] rounded-md flex items-center justify-center mr-[10px]"
          ></div>
          <div
            class="w-11 h-10 bg-[#EBEFF3] rounded-md flex items-center justify-center mr-[10px]"
          ></div>
          <div
            class="w-11 h-10 bg-[#EBEFF3] rounded-md flex items-center justify-center mr-[10px]"
          ></div>
        </div>
        <h4 class="text-xl mb-3 text-[#4F4F4F] font-bold">
          Mobil ilovani yuklab oling
        </h4>
        <div class="flex mb-[73px]">
          <div
            class="w-[188px] h-[66px] rounded-[10px] bg-[#EBEFF3] flex items-center justify-center mr-3"
          ></div>
          <div
            class="w-[188px] h-[66px] rounded-[10px] bg-[#EBEFF3] flex items-center justify-center"
          ></div>
        </div>
        <p class="text-sm text-[#9A9A9A]">
          @copy; {{ new Date().getFullYear() }} Ashyo ro’hatdan otgan
          litsenzalangan bu brend.
        </p>
      </div>
      <div class="">
        <h4 class="text-xl mb-[21px] text-[#4F4F4F] font-bold">Menyu</h4>
        <div class="max-w-[236px] flex flex-col">
          <router-link
            to="#"
            class="mb-3 text-[#4F4F4F] hover:text-black duration-200"
          >
            Ashyo haqida
          </router-link>
          <router-link
            to="#"
            class="mb-3 text-[#4F4F4F] hover:text-black duration-200"
          >
            Foydalanish shartlari
          </router-link>
          <router-link
            to="#"
            class="mb-3 text-[#4F4F4F] hover:text-black duration-200"
          >
            Mahsulotlarni va tovarlarni qaytarish siyosati
          </router-link>
          <router-link
            to="#"
            class="mb-3 text-[#4F4F4F] hover:text-black duration-200"
          >
            Biz bilan aloqa
          </router-link>
        </div>
      </div>
      <div class="">
        <h4 class="text-xl mb-[21px] text-[#4F4F4F] font-bold">Aloqa</h4>
        <a
          href="tel:+998711234567"
          class="block text-[#06172D] mb-8 text-2xl font-bold"
        >
          +998 (71) 123-45-67
        </a>
        <p class="text-[#4F4F4F] mb-3">Savolingiz bormi?</p>
        <input
          type="text"
          placeholder=" O’zingiz qiziqtirgan savollarni bering"
          class="w-[314px] border-none outline-none rounded-md py-[19px] px-[11px] bg-[#EBEFF3] text-xs placeholder:text-[ O’zingiz qiziqtirgan savollarni bering]"
        />
      </div>
    </div>
  </footer>
</template>

<style scoped></style>
