<script setup lang="ts">
import { GamesList } from "./static/js/Games.js";
import { ROMsList } from "./static/js/Games.js";
import Games from "./pages/Games1/Games.vue";
import ROMs from "./pages/ROMs/ROMs.vue";
</script>
<template>
  <div>
    <Games :Games="GamesList" />
    <!-- <ROMs :ROMs="ROMsList" /> -->
  </div>
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
