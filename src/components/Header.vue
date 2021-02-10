<template>
  <header class="header">
    <img src="../assets/img/logo.png" alt="trillo logo" class="logo" />
    <form action="#" class="search">
      <input type="text" class="search__input" placeholder="Search hotels" />
      <button class="search__button">
        search
      </button>
    </form>
  </header>
</template>

<style lang="scss" scoped>
.header {
  height: 7rem;
  background-color: #fff;
  border-bottom: var(--color-gray-lighter);
}
</style>
