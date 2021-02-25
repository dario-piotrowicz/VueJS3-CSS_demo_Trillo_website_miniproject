<template>
  <nav class="sidebar">
    <ul class="side-nav">
      <li class="side-nav__item side-nav__item--active">
        <a href="#" class="side-nav__link">
          <svg class="side-nav__icon">
            <use xlink:href="#icon-home"></use>
          </svg>
          <span>Hotel</span>
        </a>
      </li>
      <li class="side-nav__item">
        <a href="#" class="side-nav__link">
          <svg class="side-nav__icon">
            <use xlink:href="#icon-aircraft-take-off"></use>
          </svg>
          <span>Flight</span>
        </a>
      </li>
      <li class="side-nav__item">
        <a href="#" class="side-nav__link">
          <svg class="side-nav__icon">
            <use xlink:href="#icon-key"></use>
          </svg>
          <span>Car rental</span>
        </a>
      </li>
      <li class="side-nav__item">
        <a href="#" class="side-nav__link">
          <svg class="side-nav__icon">
            <use xlink:href="#icon-map"></use>
          </svg>
          <span>Tours</span>
        </a>
      </li>
    </ul>
    <div class="legal">
      &copy; 2021 by Trillo. All rights reserved.
    </div>
  </nav>
</template>

<style lang="scss" scoped>
.sidebar {
  background-color: var(--color-gray-darkest);
  flex: 0 0 18%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.side-nav {
  font-size: 1.4rem;
  list-style: none;
  margin-top: 3.5rem;

  &__item {
    position: relative;

    &:not(:last-child) {
      margin-bottom: 0.5rem;
    }

    &::before {
      content: "";
      position: absolute;
      top: 0;
      left: 0;
      height: 100%;
      width: 3px;
      background-color: var(--color-primary);
      transform: scaleY(0);
      transition: transform 0.2s, width 0.4s cubic-bezier(1, 0, 0, 1) 0.2s,
        background-color 0.1s;
    }

    &:hover::before,
    &--active::before {
      transform: scaleY(1);
      width: 100%;
    }

    &:active::before {
      background-color: var(--color-primary-lighter);
    }
  }

  &__link {
    &:link,
    &:visited {
      color: var(--color-gray-lightest);
      text-decoration: none;
      text-transform: uppercase;
      display: block;
      padding: 1.5rem 3rem;
      display: flex;
      align-items: center;
      position: relative;
    }
  }

  &__icon {
    $size: 1.75rem;
    width: $size;
    height: $size;
    margin-right: 2rem;
    fill: currentColor;
  }
}

.legal {
  font-size: 1.2rem;
  text-align: center;
  padding: 2.5rem;
  color: var(--color-gray-medium);
}
</style>
