<template>
  <app-header></app-header>
  <div class="content">
    <nav-sidebar></nav-sidebar>
    <hotel-view></hotel-view>
  </div>
</template>

<script>
import Header from "./Header";
import NavSidebar from "./NavSidebar";
import HotelView from "./HotelView";

export default {
  components: {
    "app-header": Header,
    "nav-sidebar": NavSidebar,
    "hotel-view": HotelView
  }
};
</script>
