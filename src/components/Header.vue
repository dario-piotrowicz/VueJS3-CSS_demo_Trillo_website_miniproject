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
      <div class="user-navigation__item-wrapper">
        <svg class="user-navigation__icon">
          <use xlink:href="#icon-chat"></use>
        </svg>
        <span class="user-navigation__notifications">13</span>
      </div>
      <div class="user-navigation__item-wrapper">
        <img
          src="../assets/img/user.jpg"
          alt="user profile picture"
          class="user-navigation__user-img"
        />
        <span class="user-navigation__user-name">Dario</span>
      </div>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
.header {
  font-size: 1.4rem;
  height: 7rem;
  background-color: #fff;
  border-bottom: 1px solid var(--color-gray-lighter);
  display: flex;
  justify-content: space-between;
  align-items: center;

  @media only screen and (max-width: 530px) {
    flex-wrap: wrap;
    height: 11rem;
    align-content: space-around;
  }
}

.logo {
  height: 3.25rem;
  margin-left: 2rem;
}

.search {
  flex: 0 0 40%;
  display: flex;
  justify-content: center;
  align-items: center;

  @media only screen and (max-width: 530px) {
    order: 1;
    flex: 0 0 100%;
    background-color: var(--color-gray-lighter);
  }

  &__input {
    font-family: inherit;
    font-size: inherit;
    color: inherit;
    background-color: var(--color-gray-lighter);
    border: none;
    border-radius: 50px;
    padding: 0.7rem 2rem;
    outline: none;
    width: 90%;
    transition: width 0.2s, background-color 0.2s, color 0.2s;
    margin-right: -3.25rem;

    &:focus {
      width: 100%;
      background-color: var(--color-gray-light);

      @media only screen and (max-width: 530px) {
        padding-left: 5px;
        background-color: inherit;
      }
    }

    &::placeholder {
      font-weight: 100;
      color: var(--color-gray);
    }
  }

  &__button {
    background-color: var(--color-gray-lighter);
    border: none;
    outline: none;
    transition: transform 0.05s;

    &:active {
      transform: translateY(2px);
    }
  }

  &__input + &__button {
    background-color: var(--color-gray-light);
    @media only screen and (max-width: 530px) {
      background-color: inherit;
      padding-right: 5px;
    }
  }

  &__button-icon {
    $size: 2rem;
    height: $size;
    width: $size;
    fill: var(--color-gray-dark);
  }
}

.user-navigation {
  align-self: stretch;
  display: flex;
  align-items: center;

  &__item-wrapper {
    position: relative;
    display: flex;
    align-items: center;
    padding: 0 2rem;
    cursor: pointer;
    height: 100%;

    &:hover {
      background-color: var(--color-gray-light);
    }
  }

  &__icon {
    $size: 2.25rem;
    height: $size;
    width: $size;
    fill: var(--color-gray-darker);
  }

  &__notifications {
    font-size: 0.8rem;
    $size: 1.75rem;
    height: $size;
    width: $size;
    border-radius: 50%;
    background-color: var(--color-primary);
    color: #fff;
    position: absolute;
    top: 1.5rem;
    right: 1.1rem;
    display: flex;
    justify-content: center;
    align-items: center;

    @media only screen and (max-width: 530px) {
      top: 0;
    }
  }

  &__user-img {
    $size: 3.75rem;
    height: $size;
    width: $size;
    border-radius: 50%;
    margin-right: 1rem;
  }
}
</style>
