<template>
  <main>
    <div class="main__container">
      <div class="main__container__img">
        <div class="main__container__img__text">Makina</div>
      </div>
    </div>
    <div class="main__container">
      <div class="main__container__img2">
        <div class="main__container__img2__text2">Denji</div>
      </div>
    </div>
    
  </main>
</template>
<style scoped lang="scss">
.main {
  &__container {
    &__img {
      background-image: url("../public/medias/Chainsaw-Man-Makima-2.webp");
      background-size: cover;
      height: 50em;
      &__text {
        color: white;
        font-size: 6em;
        padding: 2em;
        font-weight: 500;
      }
    }
    &__img2 {
      background-image: url("../public/medias/chainsaw-man-episode-7.png");
      background-size: cover;
      height: 50em;
      &__text2 {
        color: white;
        font-size: 6em;
        padding: 2em;
        font-weight: 500;
        padding-left: 13em;
      }
    }
  }
}


</style>
