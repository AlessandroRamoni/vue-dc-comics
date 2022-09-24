<template>
  <div class="card">
    <img :src="immagine" />
    <div id="layout">
      <p>{{ testo }}</p>
      <p id="prezzo">prezzo: {{ prezzo }}</p>
      <p id="genere">{{ genere }}</p>
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
    genere: String,
  },
};
</script>

<style scoped lang="scss">
.card {
  width: calc(100% / 6 - 25px);
  position: relative;
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
  #genere {
    color: red;
    font-size: 1em;
    position: absolute;
    top: 30px;
    right: -5px;
    transform: rotate(45deg);
    animation: colors 3s linear infinite;
    @keyframes colors {
      25% {
        color: red;
      }
      50% {
        color: green;
      }
      75% {
        color: #ffffff;
      }
      100% {
        color: rgb(240, 220, 38);
      }
    }
  }
}
</style>