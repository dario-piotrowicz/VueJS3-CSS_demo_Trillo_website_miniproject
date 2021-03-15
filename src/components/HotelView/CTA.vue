<template>
  <div class="hotel-cta">
    <h2 class="hotel-cta__text">
      Good news! We have 4 rooms for your selected dates!
    </h2>
    <button class="hotel-cta__btn">
      <span class="hotel-cta__btn-default">Book now</span>
      <span class="hotel-cta__btn-onhover">Only 4 rooms left</span>
    </button>
  </div>
</template>

<style lang="scss" scoped>
.hotel-cta {
  padding: 3.5rem 0;
  text-align: center;

  &__text {
    font-size: 2rem;
    font-weight: 300;
    text-transform: uppercase;
    margin-bottom: 2.5rem;
  }

  &__btn {
    cursor: pointer;
    outline: none;
    color: #fff;
    font-size: 1.5rem;
    font-weight: 300;
    text-transform: uppercase;
    border: none;
    border-radius: 100px;
    background-image: linear-gradient(
      to right,
      var(--color-primary-lighter),
      var(--color-primary-darker)
    );
    position: relative;
    overflow: hidden;

    &-default {
      display: inline-block;
      padding: 2rem 7.5rem;
      transition: transform 0.2s;
    }

    &-onhover {
      display: inline-block;
      height: 100%;
      width: 100%;
      padding: 2rem;
      position: absolute;
      left: 0;
      top: -100%;
      transition: top 0.2s;
    }

    &:hover {
      background-image: linear-gradient(
        to left,
        var(--color-primary-lighter),
        var(--color-primary-darker)
      );
    }

    &:hover &-default {
      transform: translateY(100%);
    }

    &:hover &-onhover {
      top: 0;
    }
  }
}
</style>
