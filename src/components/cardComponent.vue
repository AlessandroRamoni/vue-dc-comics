<template>
  <div class="card">
    <img :src="immagine" alt="" />
    <div id="layout">
      <p>{{ testo }}</p>
      <p id="prezzo">prezzo: {{ prezzo }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "cardComponent",
  props: {
    immagine: String,
    testo: String,
    prezzo: String,
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
  p {
    color: #ffffff;
  }
  #prezzo {
    color: #6a97eb;
    font-size: 0.7em;
  }
  #layout p {
    padding-top: 5px;
  }
}
</style>