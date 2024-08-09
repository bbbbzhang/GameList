<script setup lang="ts">
// import { GamesList } from "./static/js/Games.js";
import { PC_Cracks } from "./static/js/PC_Crack";
// import { ROMsList } from "./static/js/Games.js";
// import Games from "./pages/Games1/Games.vue";
import PCCCracks from "./pages/Games1/PCCCracks.vue";
// import ROMs from "./pages/ROMs/ROMs.vue";
</script>
<template>
  <div>
    <!-- <Games :Games="GamesList" /> -->
    <PCCCracks :Games="PC_Cracks" />
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
