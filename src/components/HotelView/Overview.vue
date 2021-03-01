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

  &__stars {
    margin-right: auto;
  }

  &__icon {
    &-star,
    &-location {
      $size: 1.75rem;
      width: $size;
      height: $size;
      fill: var(--color-primary);
    }
  }
}
</style>
