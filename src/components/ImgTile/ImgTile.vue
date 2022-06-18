<template>
  <div class="imgTile">
    <ImgCard :data="item" v-for="item in dataList" v-bind:key="item.id" />
  </div>
</template>

<script>
import ImgCard from "../ImgCard/ImgCard.vue";
import dataList1 from "../../hook/dataList";

export default {
  name: "ImgTile",
  components: {
    ImgCard,
  },

  setup() {
    
  },

  data() {
    return {
      dataList:[]
    };
  },

  mounted() {
    this.dataList = dataList1
  },

  methods: {},
};
</script>

<style scoped>
.imgTile {
  display: flex;
}
</style>
