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
    }
    &__img {
      grid-area: 3 / 1 / 4 / 2;
    }
    &__subsubtitle {
      grid-area: 3 / 2 / 4 / 3;
      font-size: 2em;
    }

    &__img {
      max-width: 30em;
    }
  }
}
</style>
