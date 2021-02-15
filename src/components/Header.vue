<template>
  <header class="header">
    <img src="../assets/img/logo.png" alt="trillo logo" class="logo" />
    <form action="#" class="search">
      <input type="text" class="search__input" placeholder="Search hotels" />
      <button class="search__button">
        <svg class="search__button-icon">
          <use xlink:href="#icon-magnifying-glass"></use>
        </svg>
      </button>
    </form>
    <nav class="user-navigation">
      <div class="user-navigation__item-wrapper">
        <svg class="user-navigation__icon">
          <use xlink:href="#icon-bookmark"></use>
        </svg>
        <span class="user-navigation__notifications">7</span>
      </div>
      <div class="user-navigation__item-wapper">
        <svg class="user-navigation__icon">
          <use xlink:href="#icon-chat"></use>
        </svg>
        <span class="user-navigation__notifications">13</span>
      </div>
      <div class="user-navigation__item-wrapper">
        <div class="user-navigation__user">
          <img
            src="../assets/img/user.jpg"
            alt="user profile picture"
            class="user-navigation__user-img"
          />
          <span class="user-navigation__user-name">Dario</span>
        </div>
      </div>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
.header {
  height: 7rem;
  background-color: #fff;
  border-bottom: var(--color-gray-lighter);
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  height: 3.25rem;
  margin-left: 3rem;
}

.search {
  flex: 0 0 40%;

  &__button-icon {
    $size: 2rem;
    height: $size;
    width: $size;
  }
}

.user-navigation {
  display: flex;
  align-items: center;

  &__icon {
    $size: 2.25rem;
    height: $size;
    width: $size;
  }

  &__user-img {
    $size: 3.75rem;
    height: $size;
    width: $size;
    border-radius: 50%;
  }
}
</style>
