<template>
  <header class="header">
    <wrapper class="header__wrapper wrapper">
      <div class="header__container">
        <h1 class="header__container__h1 title">Power up</h1>
        <h2 class="header__container__h2 subtitle">
          le fan site pas du tout officiel de Chainsaww man
        </h2>
      </div>
      <nav class="header__nav nav">
        <ul class="header__nav__ul navlist">
          <li class="header__nav__ul__li list">
            <NuxtLink to="/"> acceuil </NuxtLink>
          </li>
          <li class="header__nav__ul__li list">
            <NuxtLink to="/aPropos"> a propos </NuxtLink>
          </li>
          <li class="header__nav__ul__li list">
            <NuxtLink to="/contact"> nous contacter </NuxtLink>
          </li>
          <li class="header__nav__ul__li list">
            <NuxtLink to="/episodes"> liste-des-episodes </NuxtLink>
          </li>
          <li class="header__nav__ul__li list">
            <NuxtLink to="/personnages"> Personnages </NuxtLink>
          </li>
        </ul>
      </nav>
    </wrapper>
  </header>
</template>
<style lang="scss">
.header {
  background-color: #eeb314;
  color: #cf7007;
  max-width: 100%;

  &__wrapper {
    border-style: none;
  }

  &__container {
    text-align: center;

    &__h1 {
      font-size: 6em;
      margin: 0;
    }

    &__h2 {
      font-size: xx-large;
    }
  }

  &__nav {
    &__ul {
      text-align: center;
      display: flex;
      justify-content: space-around;
      font-size: large;
      list-style-type: none;
      padding: 1.5em 2em;

      :hover {
        color: bisque;
      }
      a {
        text-decoration: none;
        color: #cf7007;
        font-size: xx-large;
      }
    }
  }
}
</style>
