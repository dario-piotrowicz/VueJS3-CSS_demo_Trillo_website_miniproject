<template>
  <div class="hotel-reviews">
    <review
      text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis culpa
      molestias impedit incidunt perspiciatis illum sit qui assumenda ipsum
      corporis."
      user-name="Nick Smith"
      :user-pic-src="require('../../assets/img/user-1.jpg')"
      date="Feb 23rd, 2020"
      score="7.8"
    ></review>
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
