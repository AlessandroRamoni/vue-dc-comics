<template>
  <nav>
    <div class="container">
      <ul>
        <li>
          <a href="#"
            ><img src="../assets/img/buy-comics-digital-comics.png" alt="" /></a
          >DIGITAL COMICS
        </li>
        <li>
          <a href="#"
            ><img src="../assets/img/buy-comics-merchandise.png" alt="" /></a
          >DC MERCHANDISE
        </li>
        <li>
          <a href="#"
            ><img src="../assets/img/buy-comics-shop-locator.png" alt="" /></a
          >SUBSCRIPTION
        </li>
        <li>
          <a href="#"
            ><img src="../assets/img/buy-comics-subscriptions.png" alt="" /></a
          >COMIC SHOP LOCATOR
        </li>
        <li>
          <a href="#"
            ><img src="../assets/img/buy-dc-power-visa.svg" alt="" /></a
          >DC POWER VISA
        </li>
      </ul>
    </div>
  </nav>
</template>
 
<script>
export default {
  name: "navComponent",
};
</script>
  
<style scoped lang="scss">
nav {
  background-color: #0282f9;
}

.container {
  margin: 0 auto;
  max-width: 1000px;
}
ul {
  display: flex;
  justify-content: space-around;
}

ul li {
  display: flex;
  align-items: center;
  color: #ffffff;
  padding: 20px 0px;
  font-size: 0.7em;
}
ul li a img {
  width: 50px;
}
ul li a {
  padding-right: 10px;
}
</style>