<template>
    <section>
        <div class="container">
        <div class="card-container">
            <div class="card" v-for="card in cards" :key="card.series">{{ card.series }}
             <cardComponent />
            </div>
           
        </div>
        </div>
    </section>
</template>
 
<script>

import cardComponent from "./cardComponent.vue";

export default {
    name: "sectionComponent",
    props:{
        cards: Array
    },
    components: {
    cardComponent,
},
};
</script>
  
<style scoped lang="scss">
    $sfondoNero: #1c1c1c;
section {   
background-color: $sfondoNero;
height: 100px;
}

@mixin stileContainer {
    margin: 0 auto;
    max-width: 1000px;
    display: flex;
    align-items: center;
    justify-content: flex-start;
}

.container {
    @include stileContainer
}

h1 {
    color: #ffffff;
    font-size: 1.3em;
}

// .card-container {
//     display: flex;
// }
</style>
