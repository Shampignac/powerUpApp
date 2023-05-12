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
    <div class="arrow-container">
      <div class="left-arrow"></div>
      <div class="right-arrow"></div>
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
.arrow-container {
  display: flex;
  justify-content: space-between;
  width: 100%;
  max-width: 500px;
  margin: 0 auto;
}

.left-arrow, .right-arrow {
  width: 0;
  height: 0;
  border-top: 20px solid transparent;
  border-bottom: 20px solid transparent;
}

.left-arrow {
  border-right: 20px solid #eeb314;
}

.right-arrow {
  border-left: 20px solid #eeb314;
}

</style>
