<template>
  <div 
    class="base-beverage" 
    :style="{ backgroundColor: beverageStore.currentBase.color }"
  ></div>
</template>

<script setup lang="ts">
import { useBeverageStore } from "../stores/beverageStore";
const beverageStore = useBeverageStore();
</script>

<style scoped>
.base-beverage {
  position: relative;
  width: 100%;
  height: 100%;
  bottom: 0;
  animation: pour-tea 2s;
  z-index: 100;
}
</style>