<template>
  <div class="card">
    <img :src="data.thumb" :alt="data.series">
    <p>{{ data.series }}</p>
  </div>
</template>

<script>
export default {
    name: "cardComponent",
    props: {
      data: Object
    }
}
</script>

<style scoped lang="scss">

</style>