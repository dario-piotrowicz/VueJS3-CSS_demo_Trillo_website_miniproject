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
        <div class="user-navigation__notifications">7</div>
      </div>
      <div class="user-navigation__item-wapper">
        <svg class="user-navigation__icon">
          <use xlink:href="#icon-chat"></use>
        </svg>
        <div class="user-navigation__notifications">13</div>
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
}
</style>
