<template>
  <main>
    <div class="main__container">
      <h2 class="main__container__subtitle subtitle">épisode 1</h2>
      <h1 class="main__container__title title">le chien et la tronçonneuse</h1>
      <h3 class="main__container__subsubtitle subsubtitle">Chapitres 1</h3>
      <img
        class="main__container__img"
        src="../medias/Chainsaw-Man-Saison-1-episode-1-1600x900.jpg"
        alt=" face a face chien tronçoneuse et héros"
      />
    </div>
    <div class="main__container2">
      <h2 class="main__container2__subtitle subtitle">épisode 11</h2>
      <h1 class="main__container2__title title">arrivée a Tokyo</h1>
      <h3 class="main__container2__subsubtitle subsubtitle">
        Chapitres 2-3-4-5
      </h3>
      <img
        class="main__container__img"
        src="../medias/Chainsaw-Man-episode-2-780x439.jpg"
        alt=" face a face chien tronçoneuse et héros"
      />
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
    margin: 0 5em;
    background-image: linear-gradient(to bottom, #eeb314 250px, #f0f4f4 250px);
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: 2em 4em 1fr;
    grid-column-gap: 0px;
    grid-row-gap: 0px;

    &__subtitle {
      grid-area: 1 / 1 / 2 / 2;
      color: white;
    }
    &__title {
      grid-area: 2 / 1 / 3 / 2;
      font-weight: bolder;
      font-size: 2em;
    }
    &__img {
      grid-area: 3 / 1 / 4 / 2;
      max-width: 30em;
    }
    &__subsubtitle {
      grid-area: 3 / 2 / 4 / 3;
      font-size: 2em;
    }
  }
  &__container2 {
    margin: 1em 5em;
    background-image: linear-gradient(to bottom, #eeb314 250px, #f0f4f4 250px);
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: 2em 4em 1fr;
    grid-column-gap: 0px;
    grid-row-gap: 0px;

    &__subtitle {
      grid-area: 1 / 2 / 2 / 2;
      color: white;
    }
    &__title {
      grid-area: 2 / 2 / 3 / 2;
      font-weight: bolder;
      font-size: 2em;
    }

    &__subsubtitle {
      grid-area: 3 / 1 / 4 / 3;
      font-size: 2em;
    }

    &__img {
      grid-area: 1 / 2 / 4 / 3;
      max-width: 30em;
      margin-left: 1em;
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

.left-arrow,
.right-arrow {
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
