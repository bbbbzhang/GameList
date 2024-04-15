<template>
  <div>
    <Arcade :Arcade="ROMs['FBNeo_Arcade_Games']" />
  </div>
</template>

<script setup>
defineProps({
  ROMs: {
    type: Object,
    required: true,
  },
});
// export default {
//   mounted() {
//     console.log(111);
//   },
// };
import Arcade from "./components/Arcade.vue";
</script>

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
