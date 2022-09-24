<template>
  <div class="card">
    <img :src="immagine" alt="" />
  </div>
</template>

<script>
export default {
  name: "cardComponent",
  props: {
    immagine: String,
  },
};
</script>

<style scoped lang="scss">
.card {
  width: calc(100% / 6 - 25px);
  img {
    width: 150px;
    height: 150px;
  }
}
</style>