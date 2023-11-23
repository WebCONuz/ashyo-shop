<script setup lang="ts">
import UIBtn from "../ui/btn/UIBtn.vue";
</script>

<template>
  <section class="banner pb-[150px]">
    <div class="container">
      <div class="flex bg-[#282828] rounded-[10px]">
        <div class="w-1/2 relative">
          <img
            class="absolute right-0 top-0"
            src="../../assets/images/headphone.png"
            alt="banner"
          />
        </div>
        <div class="w-1/2 pt-[97px] pb-[134px]">
          <h3
            class="text-white text-[32px] leading-[38px] font-bold max-w-[438px] mb-[21px]"
          >
            Musiqa zavqini his qilish uchun ko'p mablag' sarflash shart emas!
          </h3>
          <UIBtn class="bg-white">
            <p class="w-[129px] py-1 text-[#111]">Batafsil</p>
          </UIBtn>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped></style>
