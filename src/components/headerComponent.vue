<template>
  <header>
    <div id="contenitore-immagine">
      <img src="../assets/img/dc-logo.png" alt="" />
    </div>
    <div id="contenitore-opzioni">
      <ul id="opzioni">
        <li>CHARACTERS</li>
        <li>COMICS</li>
        <li>MOVIES</li>
        <li>TV</li>
        <li>GAMES</li>
        <li>COLLECTIBLES</li>
        <li>VIDEOS</li>
        <li>FANS</li>
        <li>NEWS</li>
        <li>SHOP</li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "headerComponent",
};
</script>

<style scoped lang="scss">
header {
  background-color: red;
  height: 150px;
  display: flex;
  justify-content: space-between;
}
#contenitore-immagine {
 line-height: 10px;
}
#contenitore-opzioni{
  line-height: 150px;
}
#opzioni {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
}
#opzioni li {
   padding-right: 20px;
   font-size: 0.8em;
}

</style>
