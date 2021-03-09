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
      <li class="hotel-description__list-item">Close to the beach</li>
      <li class="hotel-description__list-item">Breakfast included</li>
      <li class="hotel-description__list-item">Free airport shuttle</li>
      <li class="hotel-description__list-item">Free wifi in all rooms</li>
      <li class="hotel-description__list-item">Air conditioning and heating</li>
      <li class="hotel-description__list-item">Petes allowed</li>
      <li class="hotel-description__list-item">We speak only english</li>
      <li class="hotel-description__list-item">Perfect for families</li>
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
}
</style>
