<template>
  <footer class="footer">
    <div class="footer__container">
      <h1 class="footer__container__title title">Power up</h1>
    </div>
    <wrapper class="footer__wrapper wrapper">
      <nav class="footer__nav">
        <ul class="footer__nav__ul">
          <li class="footer__nav__ul__li">
            <NuxtLink to="/"> acceuil </NuxtLink>
          </li>
          <li class="footer__nav__ul__li">
            <NuxtLink to="/aPropos"> a propos </NuxtLink>
          </li>
          <li class="footer__nav__ul__li">
            <NuxtLink to="/contact"> nous contacter </NuxtLink>
          </li>
          <li class="footer__nav__ul__li">
            <NuxtLink to="/episodes"> liste-des-episodes </NuxtLink>
          </li>
          <li class="footer__nav__ul__li">
            <NuxtLink to="/personnages"> Personnages </NuxtLink>
          </li>
        </ul>
      </nav>
      <div class="footer__container2 container2">
        <img
          class="footer__container2__img"
          src="../public/medias/wp9532701.webp"
          alt="le chien tronçoneuse"
        />
      </div>
    </wrapper>
  </footer>
</template>
<style lang="scss">
.footer {
  background-color: #eeb314;
  color: #cf7007;
  max-width: 100%;
  margin: 0;

  &__wrapper {
    display: grid;
    grid-template-columns: 1fr;
    gap: 20px;

    @media (min-width: 800px) {
      grid-template-columns: 250px 30em;
    }
  }

  &__container {
    &__title {
      font-size: 5em;
      padding-left: 1em;
    }
  }

  &__nav {
    &__ul {
      text-decoration: none;
      :hover {
        color: bisque;
      }
      &__li {
        display: flex;
        flex-direction: column;
        padding: 15px 0;
        font-size: 2em;
      }
    }
  }
  &__container2 {
    display: flex;
    justify-content: center;
    align-items: flex-end;

    &__img {
      mix-blend-mode: multiply;
      max-width: 100%;
      margin-left: 30em;

      @media (max-width: 768px) {
        margin-left: 0;
      }
    }
  }
}
a {
  text-decoration: none;
  color: #cf7007;
}
</style>
