<template>
  <div class="hotel-review">
    <blockquote class="hotel-review__text">
      {{ text }}
    </blockquote>
    <div class="hotel-review__user">
      <img
        :src="userPicSrc"
        :alt="`Picture of ${userName}`"
        class="hotel-review__user-picture"
      />
      <div class="hotel-review__user-details">
        <p class="hotel-review__user-name">
          {{ userName }}
        </p>
        <p class="hotel-review__user-date">
          {{ date }}
        </p>
      </div>
      <div class="hotel-review__user-rating">{{ score }}</div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["text", "userName", "userPicSrc", "date", "score"]
};
</script>

<style lang="scss" scoped>
.hotel-review {
  background-color: #fff;
  box-shadow: 0 2rem 5rem transparentize(#000, 0.94);
  padding: 3rem;
  margin-bottom: 3.5rem;
  font-size: 1.4rem;
  position: relative;
  overflow: hidden;

  @media only screen and (max-width: 930px) {
    padding: 2rem;
    margin-bottom: 3rem;
  }

  &__text {
    position: relative;
    z-index: 3;
    margin-bottom: 2rem;
  }

  &__user {
    display: flex;
    align-items: center;

    &-details {
      margin-right: auto;
    }

    &-picture {
      $size: 4.5rem;
      height: $size;
      width: $size;
      border-radius: 50%;
      margin-right: 1.5rem;
    }

    &-name {
      font-size: 1.1rem;
      font-weight: 600;
      text-transform: uppercase;
      margin-bottom: 0.4rem;
    }

    &-date {
      font-size: 1rem;
      color: var(color-gray-dark);
    }

    &-rating {
      color: var(--color-primary);
      font-size: 2.2rem;
      font-weight: 300;
    }
  }

  &::before {
    content: "\201C";
    position: absolute;
    top: -3.2rem;
    left: -0.9rem;
    font-size: 20rem;
    font-family: sans-serif;
    line-height: 1;
    color: var(--color-gray-lighter);
    z-index: 2;
  }
}
</style>
