<template>
    <section>
        <div class="container">
        <h1>Content goes here</h1>
    </div>
    </section>
</template>
 
<script>
export default {
    name: "sectionComponent",
};
</script>
  
<style scoped lang="scss">
section {   
background-color: rgb(0, 0, 0);
height: 100px;

}
.container {
    margin: 0 auto;
    max-width: 1000px;
    display: flex;
    align-items: center;
    justify-content: flex-start;
}
h1 {
    color: #ffffff;
    font-size: 1.3em;
}
</style>
