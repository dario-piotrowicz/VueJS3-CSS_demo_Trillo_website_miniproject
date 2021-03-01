<template>
  <main class="hotel-view">
    <gallery></gallery>
    <overview></overview>
  </main>
</template>

<script>
import Gallery from "./Gallery";
import Overview from "./Overview";

export default {
  components: {
    gallery: Gallery,
    overview: Overview
  }
};
</script>

<style lang="scss" scoped>
.hotel-view {
  background-color: #fff;
  flex: 1;
}
</style>
