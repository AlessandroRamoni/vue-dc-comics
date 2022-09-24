<template>
  <div class="card">
    <img :src="immagine" />
    <div id="layout">
      <p>{{ testo }}</p>
      <p id="prezzo">{{ prezzo }}</p>
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
  #genere {
    color: #6a97eb;
    font-size: 0.7em;
  }
  #layout p {
    padding-top: 5px;
  }
  #prezzo {
    background-color: #6a97eb;
    border-radius: 50%;
    padding: 2px;
    color: red;
    font-size: 1em;
    position: absolute;
    top: 7px;
    right: 0px;
    transform: rotate(45deg);
    animation: colors 5s linear infinite;
    @keyframes colors {
      25% {
        color: red;
      }
      50% {
        color: green;
      }
      75% {
        color: red;
      }
      90% {
        color: rgb(240, 220, 38);
      }
      100% {
        color: red;
      }
    }
  }
}
</style>