<template>
  <main class="hotel-view">
    <gallery></gallery>
  </main>
</template>

<script>
import Gallery from "./Gallery";

export default {
  components: {
    gallery: Gallery
  }
};
</script>

<style lang="scss" scoped>
.hotel-view {
  background-color: #fff;
  flex: 1;
}
</style>
