<script setup lang="ts">
defineProps({
  Likes_noBuy_noCracks: {
    type: Object,
    required: true,
  },
});
</script>

<template>
  <div class="card">
    <div class="BoxPS4_PS5">
      <div class="title">{{ "Games.Likes_noBuy_noCracks" }}</div>
      <div
        class="item2"
        v-for="(item, index) in Likes_noBuy_noCracks"
        :key="index"
      >
        <div v-if="item">
          <div style="display: flex; justify-content: flex-start">
            <div style="width: 70px">chName:</div>
            <div>{{ item && item.chName }}</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card {
  /* background-color: #ccc; */
}
.title {
  font-size: 20px;
  font-weight: 700;
  padding: 5px;
  border: 2px solid #ccc;
  border-radius: 5px;
  /* min-width: 320px; */
  margin: 0 0 5px 0;
}
.item2 {
  background-color: #ccc;
  padding: 5px;
  border: 2px solid #ccc;
  /* border-bottom: 0; */
  border-radius: 5px;
  margin: 0 0 5px 0;
}
/* .item1:last-child .item2:last-child { */
/* border-bottom: 1px solid #000; */
/* } */
</style>
