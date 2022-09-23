<template>
  <div>
    <headerComponent />
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

import {products} from "./data/data.js"

export default {
  name: "App",
  data(){
    return {
      products
    }
    
  },
  components: {
    headerComponent,
    mainComponent,
    navComponent,
    sectionComponent,
    footerComponent,
  },
};
</script>

<style lang="scss">

  @import "./components/style/generics.scss";

#app {
 padding: 0;
 margin: 0;
 box-sizing: border-box;
 margin: 0 auto;
 max-width: 1000px;
 height: 100vh;
}
</style>
