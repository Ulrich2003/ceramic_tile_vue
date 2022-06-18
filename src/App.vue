<template>
  <div class="content">
    <ImgTile class="imgTile" />
    <Nav class="nav" />
  </div>
</template>

<script>
import ImgTile from "./components/ImgTile/ImgTile.vue";
import Nav from "./components/Nav/Nav.vue";

export default {
  name: "App",
  components: {
    ImgTile,
    Nav,
  },
  data() {
    return {};
  },
};
</script>

<style>
body {
  padding: 0;
  margin: 0;
  background-color: #202224;
}

.content {
  position: relative;
}

.imgTile {
  position: absolute;
  z-index: 0;
}

.nav {
  position: fixed;
  bottom: 0;
  z-index: 10;
}
</style>
