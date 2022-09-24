<template>
  <section>
    <div class="container">
      <div class="card-container">
        <CardComponent
          v-for="(card, index) in cards"
          :immagine="card.thumb"
          :testo="card.series"
          :prezzo="card.price"
          :key="index"
        />
      </div>
    </div>
  </section>
</template>
 
<script>
import CardComponent from "./cardComponent.vue";

export default {
  name: "sectionComponent",
  props: {
    cards: Array,
  },
  components: {
    CardComponent,
  },
};
</script>
  
<style scoped lang="scss">
$sfondoNero: #1c1c1c;
section {
  background-color: $sfondoNero;
  height: 500px;
  align-items: center;
}

@mixin stileContainer {
  margin: 0 auto;
  max-width: 1000px;
  display: flex;
  align-items: center;
  justify-content: flex-start;
}

.container {
  @include stileContainer();
}

.card-container {
  width: 1000px;
  padding-top: 30px;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 20px;
}
</style>
