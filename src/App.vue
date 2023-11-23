<script setup lang="ts">
import { RouterView } from "vue-router";
import Header from "@/components/partials/Header.vue";
</script>

<template>
  <div>
    <Header />
    <RouterView />
  </div>
</template>

<style scoped></style>
