<script setup lang="ts">
defineProps({
  PC: {
    type: Object,
    required: true,
  },
});
</script>

<template>
  <div class="card">
    <div class="box_PC">
      <div class="title">{{ "Games.PC" }}</div>
      <div class="item1" v-for="(item, index) in PC" :key="index">
        <div v-if="item">
          <div class="item2" v-for="(item2, index2) in item" :key="index2">
            <div v-if="item2">
              <div style="display: flex; justify-content: flex-start">
                <div style="width: 70px">chName:</div>
                <div>{{ item2 && item2.chName }}</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card {
  /* background-color: skyblue; */
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
  background-color: skyblue;
}
/* .item1:last-child .item2:last-child { */
/* border-bottom: 1px solid #000; */
/* } */
</style>
