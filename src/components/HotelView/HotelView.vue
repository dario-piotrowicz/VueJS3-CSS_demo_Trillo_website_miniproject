<template>
  <main class="hotel-view">
    <gallery></gallery>
    <overview></overview>
    <div class="hotel-view__main-content">
      <div class="hotel-description-wrapper">
        Description
      </div>
      <div class="hotel-reviews-wrapper">
        reviews
      </div>
    </div>
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

  &__main-content {
    display: flex;
    padding: 4.5rem;
    background-color: var(--color-gray-lightest);
    border-bottom: 1px solid var(--color-gray-lighter);
  }

  .hotel-description-wrapper {
    flex: 0 0 60%;
    margin-right: 4.5rem;
  }

  .hotel-reviews-wrapper {
    flex: 1;
  }
}
</style>
