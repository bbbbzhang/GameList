<script setup lang="ts">
defineProps({
  Games: {
    type: Object,
    required: true,
  },
});
import BoxPCCracks from "./components/BoxPCCracks.vue";
</script>
<template>
  <BoxPCCracks :PC_Cracks="Games" />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
