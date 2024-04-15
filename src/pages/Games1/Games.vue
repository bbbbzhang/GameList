<script setup lang="ts">
defineProps({
  Games: {
    type: Object,
    required: true,
  },
});
import BoxPC from "./components/BoxPC.vue";
import BoxPCCracks from "./components/BoxPCCracks.vue";
import BoxPS4_PS5 from "./components/BoxPS4_PS5.vue";
import BoxLikes_noBuy_noCracks from "./components/BoxLikes_noBuy_noCracks.vue";
</script>
<template>
  <!-- <BoxPC :PC="Games.PC" /> -->
  <BoxPCCracks :PC_Cracks="Games.PC_Cracks" />
  <!-- <BoxPS4_PS5 :PS4_PS5="Games.PS4_PS5" /> -->
  <!-- <BoxLikes_noBuy_noCracks :Likes_noBuy_noCracks="Games.Likes_noBuy_noCracks" /> -->
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
