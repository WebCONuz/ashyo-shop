<script setup lang="ts">
import { ref } from "vue";
import UIBtn from "../ui/btn/UIBtn.vue";

import DownIcon from "../icons/DownIcon.vue";
import SearchIcon from "../icons/SearchIcon.vue";
import CompareIcon from "../icons/CompareIcon.vue";
import HeartIcon from "../icons/HeartIcon.vue";
import CartIcon from "../icons/CartIcon.vue";
import UserIcon from "../icons/UserIcon.vue";
import LocationIcon from "../icons/LocationIcon.vue";
import ActionIcon from "../icons/ActionIcon.vue";
import PhoneIcon from "../icons/PhoneIcon.vue";
import CleanerIcon from "../icons/CleanerIcon.vue";
import TvIcon from "../icons/TvIcon.vue";
import ConditionerIcon from "../icons/ConditionerIcon.vue";
import LaptopIcon from "../icons/LaptopIcon.vue";
import FreezIcon from "../icons/FreezIcon.vue";
import ClothmachineIcon from "../icons/ClothmachineIcon.vue";

const categoryOpen = ref<boolean>(false);

function openSubMebu(e: any) {
  if (e.target.classList.contains("sub_menu")) {
    categoryOpen.value = false;
  }
}
</script>

<template>
  <header class="header">
    <!-- 1 -->
    <div class="container py-3 bg-[#EBEFF3] flex justify-between">
      <div class="flex">
        <div
          class="flex mr-[28px] text-[#545D6A] hover:text-black duration-200 cursor-pointer"
        >
          <LocationIcon class="mr-[11px]" />
          <span to="#" class="text-sm">Tashkent</span>
        </div>
        <router-link
          to="#"
          class="text-sm text-[#545D6A] hover:text-black duration-200 mr-[15px]"
        >
          About Us
        </router-link>
        <router-link
          to="#"
          class="text-sm text-[#545D6A] hover:text-black duration-200 mr-[15px]"
        >
          Products
        </router-link>
        <router-link
          to="#"
          class="text-sm text-[#545D6A] hover:text-black duration-200 mr-[15px]"
        >
          Contacts
        </router-link>
      </div>
      <div class="flex">
        <a href="#" class="text-[#545D6A] mr-[38px] text-sm">
          +998 (71) 123-45-67
        </a>
        <div
          class="lang relative flex items-center text-[#545D6A] cursor-pointer"
        >
          <span class="w-5 mr-2 text-sm">Uz</span>
          <DownIcon />
          <div
            class="lang-submenu absolute right-0 top-[25px] z-10 bg-white rounded overflow-hidden shadow-md duration-200"
          >
            <div class="py-2 px-4 hover:bg-gray-100 duration-200 text-sm">
              Ru
            </div>
            <div class="py-2 px-4 hover:bg-gray-100 duration-200 text-sm">
              En
            </div>
            <div class="py-2 px-4 hover:bg-gray-100 duration-200 text-sm">
              Uz
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- 2 -->
    <div class="actions container">
      <div class="bg-white py-[30px] flex justify-between">
        <!-- logo -->
        <router-link to="/">
          <img
            src="../../assets/images/logo.png"
            alt="logo"
            class="w-[150px]"
          />
        </router-link>

        <!-- actions -->
        <div class="flex">
          <!-- category -->
          <div class="mr-[10px]">
            <UIBtn
              class="bg-[#134E9B] text-white font-medium"
              @click="categoryOpen = !categoryOpen"
            >
              <span class="mr-5">Kategorya</span>
              <DownIcon class="down" />
            </UIBtn>
          </div>

          <!-- search -->
          <div class="flex bg-[#EBEFF3] rounded-[6px]">
            <input
              type="text"
              class="outline-none border-none bg-[#EBEFF3] rounded-l-[6px] w-[518px] placeholder:text-gray-300 text-[13px] px-[26px]"
              placeholder="What are you looking for?"
            />
            <UIBtn class="bg-[#134E9B] text-white font-medium px-4">
              <SearchIcon />
            </UIBtn>
          </div>
        </div>

        <!-- details -->
        <div class="flex">
          <UIBtn
            class="details bg-[#EBEFF3] hover:bg-[#134E9B] duration-200 px-3 mr-3"
          >
            <CompareIcon />
          </UIBtn>
          <UIBtn
            class="details bg-[#EBEFF3] hover:bg-[#134E9B] duration-200 px-3 mr-3"
          >
            <HeartIcon />
          </UIBtn>
          <UIBtn
            class="details bg-[#EBEFF3] hover:bg-[#134E9B] duration-200 px-3 mr-3"
          >
            <CartIcon />
          </UIBtn>
          <UIBtn
            class="details bg-[#EBEFF3] hover:bg-[#134E9B] duration-200 px-3"
          >
            <UserIcon />
          </UIBtn>
        </div>
      </div>
    </div>

    <!-- 3 -->
    <nav
      class="main-nav container pb-[29px] bg-white flex items-center justify-between"
    >
      <router-link
        to="/product"
        class="text-[#545D6A] hover:text-black relative duration-200"
      >
        Aksiyalar
      </router-link>
      <router-link
        to="/product"
        class="text-[#545D6A] hover:text-black relative duration-200"
      >
        Smartfonlar
      </router-link>
      <router-link
        to="/product"
        class="text-[#545D6A] hover:text-black relative duration-200"
      >
        Noutbooklar
      </router-link>
      <router-link
        to="/product"
        class="text-[#545D6A] hover:text-black relative duration-200"
      >
        Kondetsionerlar
      </router-link>
      <router-link
        to="/product"
        class="text-[#545D6A] hover:text-black relative duration-200"
      >
        Telivizorlar
      </router-link>
      <router-link
        to="/product"
        class="text-[#545D6A] hover:text-black relative duration-200"
      >
        Muzlatgichlar
      </router-link>
      <router-link
        to="/product"
        class="text-[#545D6A] hover:text-black relative duration-200"
      >
        Kiryuvish mashinalari
      </router-link>
      <router-link
        to="/product"
        class="text-[#545D6A] hover:text-black relative duration-200"
      >
        Telivizorlar
      </router-link>
      <router-link
        to="/product"
        class="text-[#545D6A] hover:text-black relative duration-200"
      >
        Kiryuvish mashinalari
      </router-link>
    </nav>
  </header>
  <div
    class="sub_menu container absolute left-0 z-20 w-full min-h-screen pt-[130px] duration-200"
    :class="
      categoryOpen ? 'top-0 opacity-100 visible' : 'top-6 opacity-0 invisible'
    "
    @click="openSubMebu"
  >
    <!-- category sub menu -->
    <div
      class="flex border-2 border-[#EBEFF3] w-full rounded-md overflow-hidden"
    >
      <ul class="w-[32%] py-[43px] px-[72px] bg-[#EBEFF3]">
        <li class="category flex items-center cursor-pointer py-3 mb-[14px]">
          <ActionIcon />
          <span class="text-[#545D6A] ml-[15px] duration-200"> Aksiyalar </span>
        </li>
        <li class="category flex items-center cursor-pointer py-3 mb-[14px]">
          <PhoneIcon />
          <span class="text-[#545D6A] ml-[15px] duration-200">
            Smartfonlar va Aksasuerlar
          </span>
        </li>
        <li class="category flex items-center cursor-pointer py-3 mb-[14px]">
          <CleanerIcon />
          <span class="text-[#545D6A] ml-[15px] duration-200">
            Kiryuvish mashinalari
          </span>
        </li>
        <li class="category flex items-center cursor-pointer py-3 mb-[14px]">
          <TvIcon />
          <span class="text-[#545D6A] ml-[15px] duration-200">
            Telivizorlar
          </span>
        </li>
        <li class="category flex items-center cursor-pointer py-3 mb-[14px]">
          <ConditionerIcon />
          <span class="text-[#545D6A] ml-[15px] duration-200">
            Kondetsionerlar
          </span>
        </li>
        <li class="category flex items-center cursor-pointer py-3 mb-[14px]">
          <LaptopIcon />
          <span class="text-[#545D6A] ml-[15px] duration-200">
            Kompuyert va jihozlari
          </span>
        </li>
        <li class="category flex items-center cursor-pointer py-3 mb-[14px]">
          <FreezIcon />
          <span class="text-[#545D6A] ml-[15px] duration-200">
            Muzlatgichlar
          </span>
        </li>
        <li class="category flex items-center cursor-pointer py-3">
          <ClothmachineIcon />
          <span class="text-[#545D6A] ml-[15px] duration-200">
            Kir yuvish mashinalari
          </span>
        </li>
      </ul>
      <div class="w-[68%] py-[43px] px-[72px] bg-white">
        <div class="w-full h-full overflow-y-auto flex gap-x-4">
          <div class="w-1/3 flex flex-col">
            <h3 class="font-medium mb-[25px]">Smartfonlar</h3>
            <router-link
              to="#"
              class="text-[#545D6A] text-sm mb-[17px] hover:text-[#454545] duration-200"
            >
              Oppo smartfonlar
            </router-link>
            <router-link
              to="#"
              class="text-[#545D6A] text-sm mb-[17px] hover:text-[#454545] duration-200"
            >
              Oppo smartfonlar
            </router-link>
            <router-link
              to="#"
              class="text-[#545D6A] text-sm mb-[17px] hover:text-[#454545] duration-200"
            >
              Vivo smartfonlar
            </router-link>
            <router-link
              to="#"
              class="text-[#545D6A] text-sm mb-[17px] hover:text-[#454545] duration-200"
            >
              Realmi smartfonlar
            </router-link>
            <router-link
              to="#"
              class="text-[#545D6A] text-sm mb-[17px] hover:text-[#454545] duration-200"
            >
              Redmi smartfonlar
            </router-link>
            <router-link
              to="#"
              class="text-[#545D6A] text-sm mb-[17px] hover:text-[#454545] duration-200"
            >
              Xiaomi smartfonlar
            </router-link>
            <router-link
              to="#"
              class="text-[#545D6A] text-sm mb-[17px] hover:text-[#454545] duration-200"
            >
              Artel smartfonlar
            </router-link>
            <router-link
              to="#"
              class="text-[#545D6A] text-sm mb-[17px] hover:text-[#454545] duration-200"
            >
              Samsung smartfonlar
            </router-link>
            <router-link
              to="#"
              class="text-[#545D6A] text-sm mb-[17px] hover:text-[#454545] duration-200"
            >
              Iphone smartfonlar
            </router-link>
            <router-link
              to="#"
              class="text-[#545D6A] text-sm mb-[17px] hover:text-[#454545] duration-200"
            >
              Nokia smartfonlar
            </router-link>
          </div>
          <div class="w-1/3 flex flex-col">
            <h3 class="font-medium mb-[25px]">Telfon aksesurlari</h3>
            <router-link
              to="#"
              class="text-[#545D6A] text-sm mb-[17px] hover:text-[#454545] duration-200"
            >
              Quvvatlagich
            </router-link>
            <router-link
              to="#"
              class="text-[#545D6A] text-sm mb-[17px] hover:text-[#454545] duration-200"
            >
              Telfon g’iloflari
            </router-link>
            <router-link
              to="#"
              class="text-[#545D6A] text-sm mb-[17px] hover:text-[#454545] duration-200"
            >
              Quloqchinlar
            </router-link>
            <router-link
              to="#"
              class="text-[#545D6A] text-sm mb-[17px] hover:text-[#454545] duration-200"
            >
              Xotira chiplari
            </router-link>
            <router-link
              to="#"
              class="text-[#545D6A] text-sm mb-[17px] hover:text-[#454545] duration-200"
            >
              Ekran himoya oynasi
            </router-link>
          </div>
          <div class="w-1/3"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
path {
  transition: all 0.2s;
}
.down path {
  stroke: white;
}
.details path {
  transition: all 0.3s;
}
.details:hover path {
  stroke: transparent;
  fill: #fff;
}
.lang .lang-submenu {
  opacity: 0;
  visibility: hidden;
}
.lang:hover .lang-submenu {
  opacity: 1;
  visibility: visible;
}
.category:hover path {
  stroke: #454545;
}
.category:hover span {
  color: #454545;
}
.main-nav a::before {
  content: "";
  position: absolute;
  bottom: -4px;
  left: 0;
  height: 1.5px;
  background: #000;
  width: 0;
  transition: 0.2s;
}
.main-nav a:hover::before {
  width: 100%;
}
</style>
