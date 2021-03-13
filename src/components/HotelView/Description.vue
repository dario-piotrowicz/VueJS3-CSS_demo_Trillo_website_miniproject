<template>
  <div class="hotel-description">
    <p class="hotel-description__paragraph">
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Repellendus
      dicta earum, pariatur, illo dolore incidunt quod recusandae possimus
      quisquam fuga omnis aliquam adipisci velit rerum nobis laborum! Quod,
      obcaecati sequi. Veniam quia quasi non molestias?
    </p>
    <p class="hotel-description__paragraph">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus magnam
      nostrum, similique earum culpa vitae commodi nam ratione cum autem.
    </p>
    <ul class="hotel-description__list">
      <li class="hotel-description__list-item">
        <svg class="hotel-description__list-item-icon">
          <use xlink:href="#icon-chevron-thin-right"></use>
        </svg>
        <span class="hotel-description__list-item-text">
          Close to the beach
        </span>
      </li>
      <li class="hotel-description__list-item">
        <svg class="hotel-description__list-item-icon">
          <use xlink:href="#icon-chevron-thin-right"></use>
        </svg>
        <span class="hotel-description__list-item-text">
          Breakfast included
        </span>
      </li>
      <li class="hotel-description__list-item">
        <svg class="hotel-description__list-item-icon">
          <use xlink:href="#icon-chevron-thin-right"></use>
        </svg>
        <span class="hotel-description__list-item-text">
          Free airport shuttle
        </span>
      </li>
      <li class="hotel-description__list-item">
        <svg class="hotel-description__list-item-icon">
          <use xlink:href="#icon-chevron-thin-right"></use>
        </svg>
        <span class="hotel-description__list-item-text">
          Free wifi in all rooms
        </span>
      </li>
      <li class="hotel-description__list-item">
        <svg class="hotel-description__list-item-icon">
          <use xlink:href="#icon-chevron-thin-right"></use>
        </svg>
        <span class="hotel-description__list-item-text">
          Air conditioning and heating
        </span>
      </li>
      <li class="hotel-description__list-item">
        <svg class="hotel-description__list-item-icon">
          <use xlink:href="#icon-chevron-thin-right"></use>
        </svg>
        <span class="hotel-description__list-item-text">
          Petes allowed
        </span>
      </li>
      <li class="hotel-description__list-item">
        <svg class="hotel-description__list-item-icon">
          <use xlink:href="#icon-chevron-thin-right"></use>
        </svg>
        <span class="hotel-description__list-item-text">
          We speak only english
        </span>
      </li>
      <li class="hotel-description__list-item">
        <svg class="hotel-description__list-item-icon">
          <use xlink:href="#icon-chevron-thin-right"></use>
        </svg>
        <span class="hotel-description__list-item-text">
          Perfect for families
        </span>
      </li>
    </ul>
    <div class="hotel-description__recommendations">
      <p class="hote-description__recommendations-counter">
        Lucy and 3 other friends reccomend this hotel.
      </p>
      <div class="hotel-description__recommendations-friends">
        <img
          src="../../assets/img/friend-1.jpg"
          alt="friend 1"
          class="hotel-description__recommendations-friend-img"
        /><img
          src="../../assets/img/friend-2.jpg"
          alt="friend 2"
          class="hotel-description__recommendations-friend-img"
        /><img
          src="../../assets/img/friend-3.jpg"
          alt="friend 3"
          class="hotel-description__recommendations-friend-img"
        /><img
          src="../../assets/img/friend-4.jpg"
          alt="friend 4"
          class="hotel-description__recommendations-friend-img"
        />
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.hotel-description {
  width: 100%;
  background-color: #fff;
  box-shadow: 0 2rem 5rem transparentize(#000, 0.94);
  padding: 3rem;
  font-size: 1.4rem;

  &__paragraph {
    &:not(:last-of-type) {
      margin-bottom: 2rem;
    }
  }

  &__list {
    list-style: none;
    margin: 3rem 0;
    padding: 3rem 0;
    border-top: 1px solid var(--color-gray-lighter);
    border-bottom: 1px solid var(--color-gray-lighter);
    display: flex;
    flex-wrap: wrap;

    &-item {
      flex: 0 0 50%;
      margin-bottom: 0.7rem;

      &-icon {
        $size: 1rem;
        width: $size;
        height: $size;
        margin-right: 0.7rem;
        fill: var(--color-primary);
      }
    }
  }
}
</style>
