<script setup lang="ts">
import { RouterView } from "vue-router";
import Header from "@/components/partials/Header.vue";
import Footer from "@/components/partials/Footer.vue";
</script>

<template>
  <div>
    <Header />
    <RouterView />
    <Footer />
  </div>
</template>

<style scoped></style>
