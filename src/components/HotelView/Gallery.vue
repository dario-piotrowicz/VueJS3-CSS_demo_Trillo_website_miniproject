<template>
  <div class="gallery">
    <figure class="gallery__item">
      <img
        src="../../assets/img/hotel-1.jpg"
        alt="Hotel, pool at night"
        class="gallery__photo"
      />
    </figure>
    <figure class="gallery__item">
      <img
        src="../../assets/img/hotel-2.jpg"
        alt="Hotel, pool during the day"
        class="gallery__photo"
      />
    </figure>
    <figure class="gallery__item">
      <img
        src="../../assets/img/hotel-3.jpg"
        alt="Scenery"
        class="gallery__photo"
      />
    </figure>
  </div>
</template>

<style lang="scss" scoped>
.gallery {
  display: flex;

  &__photo {
    display: block;
    width: 100%;
  }
}
</style>
