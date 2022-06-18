<template>
  <div class="imgTile">
    <ImgCard :data="item" v-for="item in dataList" v-bind:key="item.id" />
  </div>
</template>

<script>
import ImgCard from "../ImgCard/ImgCard.vue";
import dataList from "../../hook/dataList";

export default {
  name: "ImgTile",
  components: {
    ImgCard,
  },
  setup() {
    return {
      dataList: dataList(),
    };
  },
};
</script>

<style scoped>
.imgTile {
  display: flex;
  flex-wrap: wrap;
}
</style>
