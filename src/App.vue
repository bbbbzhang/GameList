<script setup lang="ts">
import BoxPC from "./components/BoxPC.vue";
import BoxPCCracks from "./components/BoxPCCracks.vue";
import { Games } from "./static/js/Games";
</script>
<template>
  <BoxPC :PC="Games.PC" />
  <BoxPCCracks :PC_Cracks="Games.PC_Cracks" />
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
