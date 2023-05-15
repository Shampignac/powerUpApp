<template>
  <main class="main">
    <div class="carousel-wrapper">
      <div class="carousel-container">
        <div class="carousel">
          <div class="image-one"></div>
          <div class="image-two"></div>
          <div class="image-three"></div>
        </div>
      </div>
    </div>
    <div class="main__container">
      <h2 class="main__container__subtitle subtitle">Dernier épisode</h2>
      <h1 class="main__container__title title">Katana VS tronçonneuse</h1>
      <h3 class="main__container__subsubtitle subsubtitle">
        Chapitres 35-36-37-38-40
      </h3>
      <img
        class="main__container__img"
        src="/medias/Chainsaw-Man-episode-12-1600x900.jpg"
        alt=" combat tronçonneuse VS katana"
      />
    </div>
  </main>
</template>

<style scoped lang="scss">
$size-width: 1300px;
$size-height: 500px;

.carousel-wrapper {
  width: cover;
  height: $size-height * 1.4;
  display: flex;
  justify-content: center;
  align-items: center;
  box-shadow: 5px 5px 25px 0px rgba(46, 61, 73, 0.2);
  border-radius: 20px;
  margin: 100px auto 20px;
}

.carousel-container {
  width: $size-width;
  height: $size-height;
  overflow: hidden;
  margin: 0 auto;
}

.carousel {
  display: flex;
  width: $size-width * 3;
  animation: sliding 12s infinite;
  div {
    width: $size-width;
    height: $size-height;
    background-size: cover;
    background-position: center;
  }
  &:hover {
    animation-play-state: paused;
  }
  .image-one {
    background-image: url("../public/medias/Chainsaw-Man-episode-12-1600x900.jpg");
  }
  .image-two {
    background-image: url("../public/medias/Chainsaw-Man-episode-2-780x439.jpg");
  }
  .image-three {
    background-image: url("../public/medias/chainsaw-man-episode-7.png");
  }
}

@keyframes sliding {
  30% {
    transform: translateX(0);
  }
  35% {
    transform: translateX(-$size-width);
  }
  65% {
    transform: translateX(-$size-width);
  }
  70% {
    transform: translateX(-$size-width * 2);
  }
  98% {
    transform: translateX(-$size-width * 2);
  }
  100% {
    transform: translateX(0);
  }
}

@media screen and (max-width: 768px) {
  $size-width: 240px;
  $size-height: 150px;
  .carousel-wrapper {
    width: $size-width * 1.3;
    height: $size-height * 1.4;
  }

  .carousel-container {
    width: $size-width;
    height: $size-height;
  }

  .carousel {
    width: $size-width * 3;
    > div {
      width: $size-width;
      height: $size-height;
    }
  }

  @keyframes sliding {
    30% {
      transform: translateX(0);
    }
    35% {
      transform: translateX(-$size-width);
    }
    65% {
      transform: translateX(-$size-width);
    }
    70% {
      transform: translateX(-$size-width * 2);
    }
    98% {
      transform: translateX(-$size-width * 2);
    }
    100% {
      transform: translateX(0);
    }
  }
}

.main {
  max-width: 100%;

  &__container {
    margin: 0 5em;
    background-image: linear-gradient(to bottom, #eeb314 250px, #f0f4f4 250px);
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: 2em 4em 1fr;
    grid-column-gap: 0px;
    grid-row-gap: 40px;

    &__subtitle {
      grid-area: 1 / 1 / 2 / 2;
      color: white;
      font-size: 3em;
    }
    &__title {
      grid-area: 2 / 1 / 3 / 2;
      font-weight: bolder;
      font-size: 2em;
    }
    &__img {
      grid-area: 3 / 1 / 4 / 2;
      max-width: 50em;
      justify-self: end;
      padding-left: 2em;
      padding-bottom: 4em;
    }
    &__subsubtitle {
      grid-area: 2 / 3 / 4 / 3;
      font-size: 3em;
    }
  }
}
@media screen and (max-width: 767px) {
  .main {
    &__container {
      margin: 0 1em;
      grid-template-columns: 1fr;
      grid-template-rows: 2em 4em auto 1fr;
      grid-template-areas:
        "subtitle"
        "title"
        "img"
        "subsubtitle";
      &__subtitle {
        grid-area: subtitle;
      }
      &__title {
        grid-area: title;
      }
      &__img {
        grid-area: img;
        max-width: 100%;
      }
      &__subsubtitle {
        grid-area: subsubtitle;
      }
    }
  }
}
</style>

<script></script>
