<template>
  <nav class="sidebar">
    <ul class="side-nav">
      <li class="side-nav__item">
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
  &__icon {
    $size: 1.75rem;
    width: $size;
    height: $size;
  }
}

.legal {
  font-size: 1.2rem;
  text-align: center;
  padding: 2.5rem;
  color: var(--color-gray-medium);
}
</style>
