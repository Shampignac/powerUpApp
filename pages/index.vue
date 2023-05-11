<template>
  <main class="main">
    <Carousel>
      <Slide v-for="image in images" :key="image.id">
        <div class="carousel__item">
          <img :src="image.src" :alt="image.alt" />
        </div>
      </Slide>

      <template #addons>
        <Navigation />
        <Pagination />
      </template>
    </Carousel>
    <div class="main__container">
      <h2 class="main__container__subtitle subtitle">Dernier épisode</h2>
      <h1 class="main__container__title title">Katan VS tronçonneuse</h1>
      <h3 class="main__container__subsubtitle subsubtitle">
        Chapitres 35-36-37-38-40
      </h3>
      <img
        class="main__container__img"
        src="../medias/Chainsaw-Man-episode-12-1600x900.jpg"
        alt=" combat tronçonneuse VS katana"
      />
    </div>
  </main>
</template>

<style scoped lang="scss">
.carousel__item {
  font-size: 20px;
  border-radius: 8px;
}

.carousel__slide {
  padding: 10px;
}

.carousel__prev,
.carousel__next {
  box-sizing: content-box;
  border: 5px solid white;
}
.main {
  max-width: 100%;
  margin: 0;

  &__container {
    margin: 0 5em;
    background-image: linear-gradient(to bottom, #eeb314 250px, #f0f4f4 250px);
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: 2em 4em 1fr;
    grid-column-gap: 0px;
    grid-row-gap: 0px;
    &__subtitle {
      grid-area: 1 / 1 / 2 / 2;
    }
    &__title {
      grid-area: 2 / 1 / 3 / 2;
    }
    &__img {
      grid-area: 3 / 1 / 4 / 2;
    }
    &__subsubtitle {
      grid-area: 3 / 2 / 4 / 3;
    }

    &__img {
      max-width: 30em;
    }
  }
}
</style>

<script>
import { defineComponent } from "vue";
import { Carousel, Navigation, Pagination, Slide } from "vue3-carousel";

import "vue3-carousel/dist/carousel.css";

export default defineComponent({
  name: "Basic",
  components: {
    Carousel,
    Slide,
    Pagination,
    Navigation,
  },
  data() {
    return {
      images: [
        {
          id: 1,
          src: "medias/55722-Power-Chainsaw-ManPower-Chainsaw-Man-HD-Wallpaper.jpg",
          alt: "Power personnage",
        },
        {
          id: 2,
          src: "medias/aki-Chainsawman.jpg",
          alt: "Image 2 alt text here",
        },
        {
          id: 3,
          src: "medias/Chainsaw-Man-episode-2-780x439.jpg",
          alt: "Image 3 alt text here",
        },
      ],
    };
  },
});
</script>
