<template>
  <div class="imgCard">
    <img :src="data.src">
    <p>{{data.content}}</p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    data: Object
  },
  data(){
    return {

    }
  }
}
</script>

<style scoped>
.imgCard{
    width: calc(100vw/3);
    height: 20rem;
    overflow: hidden;
    position: relative;
}
.imgCard img{
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: 0.5s;
    position: absolute;
    z-index: 10;
}

.imgCard img:hover{
    transform: scale(1.2);
}

.imgCard p{
    position: absolute;
    z-index: 20;
    bottom: 1.2rem;
    left: 1.1rem;
    right: 1.1rem;
    color: #fff;
    font-family: Arial, Helvetica, sans-serif;
    font-size: small;
    text-shadow: #000 1px 0 0, #000 0 1px 0, #000 -1px 0 0, #000 0 -1px 0;
}
</style>
