<template>
  <div class="hotel-reviews">
    <review></review>
  </div>
</template>

<script>
import Review from "./Review";

export default {
  components: {
    review: Review
  }
};
</script>

<style lang="scss" scoped>
.hotel-reviews {
}
</style>
