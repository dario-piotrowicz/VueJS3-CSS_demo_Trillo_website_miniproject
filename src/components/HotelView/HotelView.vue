<template>
  <main class="hotel-view">
    <gallery></gallery>
    <overview></overview>
    <div class="hotel-view__main-content">
      <div class="hotel-description-wrapper">
        <description></description>
      </div>
      <div class="hotel-reviews-wrapper">
        <reviews></reviews>
      </div>
    </div>
    <cta></cta>
  </main>
</template>

<script>
import Gallery from "./Gallery";
import Overview from "./Overview";
import Description from "./Description";
import Reviews from "./Reviews";
import CTA from "./CTA";

export default {
  components: {
    gallery: Gallery,
    overview: Overview,
    description: Description,
    reviews: Reviews,
    cta: CTA
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

    @media only screen and (max-width: 930px) {
      padding: 2rem;
    }
    @media only screen and (max-width: 600px) {
      flex-direction: column;
    }
  }

  .hotel-description-wrapper {
    flex: 0 0 60%;
    margin-right: 4.5rem;

    @media only screen and (max-width: 930px) {
      margin-right: 2rem;
    }
    @media only screen and (max-width: 600px) {
      margin-right: 0;
      margin-bottom: 3rem;
    }
  }

  .hotel-reviews-wrapper {
    flex: 1;

    @media only screen and (max-width: 600px) {
      margin-bottom: 3rem;
    }
  }
}
</style>
