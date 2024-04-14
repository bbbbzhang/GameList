<script setup lang="ts">
defineProps({
  PC_Cracks: {
    type: Object,
    required: true,
  },
});
</script>

<template>
  <div class="card">
    <div class="box_PC_Cracks">
      <div class="title">
        {{ "Games.PC_Cracks" }}
      </div>
      <div class="item1" v-for="(item, index) in PC_Cracks" :key="index">
        <div v-if="item">
          <div class="item2" v-for="(item2, index2) in item" :key="index2">
            <div v-if="item2">
              <div style="display: flex; justify-content: flex-start">
                <div style="width: 70px">chName:</div>
                <div>{{ item2 && item2.chName }}</div>
              </div>
              <div style="display: flex; justify-content: flex-start">
                <div style="width: 70px">path1:</div>
                <div>{{ item2 && item2.path1 }}</div>
              </div>
              <div style="display: flex; justify-content: flex-start">
                <div style="width: 70px">path2:</div>
                <div>{{ item2 && item2.path2 }}</div>
              </div>
              <div style="display: flex; justify-content: flex-start">
                <div style="width: 70px">version:</div>
                <div>{{ item2 && item2.version }}</div>
              </div>
              <div style="display: flex; justify-content: flex-start">
                <div style="width: 70px">platform:</div>
                <div>{{ item2 && item2.platform }}</div>
              </div>
              <div style="display: flex; justify-content: flex-start">
                <div style="width: 70px">prompt:</div>
                <div>{{ item2 && item2.prompt }}</div>
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
  /* background-color: pink; */
}
.title {
  font-size: 20px;
  font-weight: 700;
  padding: 5px;
  border: 2px solid #ccc;
  border-radius: 5px;
  width: 320px;
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
