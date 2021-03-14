<template>
  <div class="hotel-review">
    <blockquote class="hotel-review__text">
      {{ text }}
    </blockquote>
    <div class="hotel-review__user">
      <img
        :src="userPicSrc"
        :alt="`Picture of ${userName}`"
        class="hotel-review__user-picture"
      />
      <div class="hotel-review__user-details">
        <p class="hotel-review__user-name">
          {{ userName }}
        </p>
        <p class="hotel-review__user-date">
          {{ date }}
        </p>
      </div>
      <div class="hotel-review__user-rating">{{ score }}</div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["text", "userName", "userPicSrc", "date", "score"]
};
</script>

<style lang="scss" scoped>
.hotel-review {
}
</style>
