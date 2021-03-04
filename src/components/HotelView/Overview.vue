<template>
  <div class="overview">
    <h1 class="overview__heading">Hotel Las Palmas</h1>
    <div class="overview__stars">
      <svg class="overview__icon-star">
        <use xlink:href="#icon-star"></use>
      </svg>
      <svg class="overview__icon-star">
        <use xlink:href="#icon-star"></use>
      </svg>
      <svg class="overview__icon-star">
        <use xlink:href="#icon-star"></use>
      </svg>
      <svg class="overview__icon-star">
        <use xlink:href="#icon-star"></use>
      </svg>
      <svg class="overview__icon-star">
        <use xlink:href="#icon-star"></use>
      </svg>
    </div>
    <div class="overview__location">
      <svg class="overview__icon-location">
        <use xlink:href="#icon-location-pin"></use>
      </svg>
      <span class="overview__location-name">Albufeira, Portugal</span>
    </div>
    <div class="overview__rating">
      <div class="overview__rating-average">8.6</div>
      <div class="overview__rating-count">429 votes</div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.overview {
  display: flex;
  align-items: center;
  border-bottom: 1px solid var(--color-gray-lighter);

  &__heading {
    font-size: 2.25rem;
    font-weight: 300;
    text-transform: uppercase;
    letter-spacing: 1px;
    padding: 1.5rem 3rem;
  }

  &__stars {
    /* this with margin-right auto is a useful
    trick that can be used with flex to create
    empty space between two elements */
    margin-right: auto;

    display: flex;
  }

  &__icon {
    &-star,
    &-location {
      $size: 1.75rem;
      width: $size;
      height: $size;
      fill: var(--color-primary);
    }

    &-location {
      margin-right: 0.5rem;
    }
  }

  &__location {
    font-size: 1.2rem;
    display: flex;
    align-items: center;

    &-name {
      color: var(--color-primary);
      border-bottom: 1px solid currentColor;
      padding: 2px;
      display: inline-block;
    }
  }
}
</style>
