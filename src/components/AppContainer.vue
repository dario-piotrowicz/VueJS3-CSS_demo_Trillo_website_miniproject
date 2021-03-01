<template>
  <div class="container">
    <app-header></app-header>
    <div class="content">
      <nav-sidebar></nav-sidebar>
      <hotel-view></hotel-view>
    </div>
  </div>
</template>

<script>
import Header from "./Header";
import NavSidebar from "./NavSidebar";
import HotelView from "./HotelView/HotelView";

export default {
  components: {
    "app-header": Header,
    "nav-sidebar": NavSidebar,
    "hotel-view": HotelView
  }
};
</script>

<style lang="scss" scoped>
.container {
  max-width: 120rem;
  margin: 8rem auto;
  background-color: var(--color-gray-lightest);
  box-shadow: 0 2rem 6rem transparentize(#000, 0.7);
}

.content {
  display: flex;
}
</style>
