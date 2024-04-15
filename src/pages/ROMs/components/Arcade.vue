<script setup>
import { ref, onMounted } from "vue";
const props = defineProps({
  Arcade: {
    type: Object,
    required: true,
  },
});
onMounted(() => {
  // console.log("Arcade", props.Arcade["Likes_Arcade_ROMs"]["items"]);
});
</script>
<template>
  <div class="card">
    <div class="BoxROMs">
      <div class="title">
        {{ "ROMs.FBNeo_Arcade_Games.Likes_Arcade_ROMs" }}
      </div>
      <div
        class="item1"
        v-for="(item, index) in props.Arcade.Likes_Arcade_ROMs.items"
        :key="index"
      >
        <div class="item2" v-if="item">
          <div style="display: flex; justify-content: flex-start">
            <div style="width: 70px">label:</div>
            <div>{{ item && item.label }}</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card {
  /* background-color: pink; */
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
  padding: 5px;
  border: 2px solid #ccc;
  /* border-bottom: 0; */
  border-radius: 5px;
  margin: 0 0 5px 0;
  background-color: pink;
}
.item1:last-child .item2:last-child {
  /* border-bottom: 1px solid #000; */
}
</style>
