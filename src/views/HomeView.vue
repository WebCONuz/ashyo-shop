<script setup lang="ts">
import Intro from "../components/partials/Intro.vue";
import LogoGrid from "../components/partials/LogoGrid.vue";
import ProductSlider from "../components/partials/ProductSlider.vue";
import CategoryGrid from "../components/partials/CategoryGrid.vue";
import ProductBanner from "../components/partials/ProductBanner.vue";
</script>

<template>
  <main class="home">
    <Intro />
    <LogoGrid />
    <ProductSlider title="Most popular product" />
    <ProductSlider title="Most popular product" />
    <ProductSlider title="Most popular product" />
    <CategoryGrid />
    <ProductSlider title="Oxirgi ko’rgan mahsulotlar" />
    <ProductBanner />
    <ProductSlider title="Aksiyadagi tovarlar" />
  </main>
</template>

<style></style>
