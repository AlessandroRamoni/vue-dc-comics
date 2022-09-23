<template>
  <header>
    <div id="contenitore-immagine">
      <img src="../assets/img/dc-logo.png" alt="" />
    </div>
    <div id="contenitore-opzioni">
      <ul id="opzioni">
        <li><a href="">CHARACTERS</a></li>
        <li><a href="">COMICS</a></li>
        <li><a href="">MOVIES</a></li>
        <li><a href="">TV</a></li>
        <li><a href="">GAMES</a></li>
        <li><a href="">COLLECTIBLES</a></li>
        <li><a href="">VIDEOS</a></li>
        <li><a href="">FANS</a></li>
        <li><a href="">NEWS</a></li>
        <li><a href="">SHOP</a></li>
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
  background-color:#ffffff;
  height: 150px;
  display: flex;
  justify-content: space-between;
  align-items: center;
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
   color: #252525;
   font-weight: 600;
}
#opzioni li:hover {
  color: #0282f9;
}
</style>
