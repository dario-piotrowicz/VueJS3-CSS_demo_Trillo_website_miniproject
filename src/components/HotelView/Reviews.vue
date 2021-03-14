<template>
  <div class="hotel-reviews">
    <review
      v-for="review in reviews"
      :key="review.id"
      :text="review.text"
      :user-name="review.userName"
      :user-pic-src="review.userPicSrc"
      :date="review.date"
      :score="review.score"
    ></review>
    <button class="hotel-reviews__show-all-btn">
      Show all
      <span class="hotel-reviews__show-all-btn-arrow">&rarr;</span>
    </button>
  </div>
</template>

<script>
import Review from "./Review";

export default {
  data: function() {
    return {
      reviews: [
        {
          id: 0,
          text: `Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis culpa
      molestias impedit incidunt perspiciatis illum sit qui assumenda ipsum
      corporis.`,
          userName: "Nick Smith",
          userPicSrc: require("../../assets/img/user-1.jpg"),
          date: "Feb 23rd, 2020",
          score: "7.8"
        },
        {
          id: 1,
          text: `Lorem ipsum dolor sit amet consectetur adipisicing elit.
      Voluptatum dicta doloremque pariatur accusantium. Incidunt, eius!`,
          userName: "Mary Thomas",
          userPicSrc: require("../../assets/img/user-2.jpg"),
          date: "Sept 13th, 2020",
          score: "9.3"
        }
      ]
    };
  },
  components: {
    review: Review
  }
};
</script>

<style lang="scss" scoped>
.hotel-reviews {
  display: flex;
  flex-direction: column;
  align-items: center;

  &__show-all-btn {
    background-color: transparent;
    color: var(--color-primary);
    border: none;
    border-bottom: 1px solid currentColor;
    padding: 2px;
    display: inline-block;
    outline: none;
    cursor: pointer;

    &-arrow {
      line-height: 1;
      font-size: 2.5rem;
      margin-left: 3px;
      transition: margin-left 0.2s;
    }

    &:hover &-arrow {
      margin-left: 8px;
    }
  }
}
</style>
