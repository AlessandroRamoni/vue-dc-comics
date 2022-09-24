<template>
  <div id="app">
    <headerComponent />
    <herobanner-component />
    <sectionComponent :cards="products" />
    <navComponent />
    <mainComponent />
    <footerComponent />
  </div>
</template>

<script>
import headerComponent from "./components/headerComponent.vue";
import mainComponent from "./components/mainComponent.vue";
import sectionComponent from "./components/sectionComponent.vue";
import navComponent from "./components/navComponent.vue";
import footerComponent from "./components/footerComponent.vue";

import { products } from "./data/data.js";
import HerobannerComponent from "./components/herobannerComponent.vue";

export default {
  name: "App",
  data() {
    return {
      products,
    };
  },
  components: {
    headerComponent,
    mainComponent,
    navComponent,
    sectionComponent,
    footerComponent,
    HerobannerComponent,
  },
};
</script>

<style lang="scss">
@import "./components/style/generics.scss";
@import url("https://fonts.googleapis.com/css2?family=Luckiest+Guy&display=swap");
#app {
  font-family: "Luckiest Guy", cursive;
}
</style>
