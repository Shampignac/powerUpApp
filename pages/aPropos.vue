<template>
  <main>
    <div class="main__container container">
      <H1 class="main__container__title"> a propos</H1>
      <div class="parallax"></div>
      <p class="main__container__text text">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin cursus
        eget orci ut pulvinar. Fusce rutrum purus eu augue pellentesque mattis.
        Duis ullamcorper sodales sagittis. Donec tristique, lacus sit amet
        tempus fringilla, eros metus condimentum ante, in pellentesque erat
        tortor et ex. Quisque et dignissim lectus. Praesent vehicula placerat
        scelerisque. Fusce eget cursus velit. Vestibulum eu mi volutpat, finibus
        arcu in, feugiat tellus. In neque lacus, rutrum vel ultricies a, finibus
        et odio. Donec a tortor sed eros convallis elementum quis blandit purus.
        Duis pellentesque aliquam elit non feugiat. Quisque at faucibus turpis.
        Nullam dolor magna, fermentum nec aliquet nec, lobortis in leo. Nunc
        luctus urna id pulvinar gravida. In et porttitor massa, bibendum
        convallis urna. Fusce eu odio mattis, dignissim urna quis, fringilla
        diam. Suspendisse mattis lacus quis vulputate hendrerit. In at sodales
        mauris. Nam dignissim ligula ligula, vel blandit neque commodo a. Nam
        quis lacus magna. Praesent viverra risus sit amet vestibulum tristique.
        Sed nec turpis consectetur, pharetra dui eget, porttitor elit. Duis
        blandit tempus elit, ut iaculis sapien pellentesque non. Sed ac eros
        tincidunt, vulputate odio a, pretium leo. Pellentesque gravida rhoncus
        auctor. Donec sit amet viverra nisl, quis posuere urna.
      </p>
    </div>
  </main>
</template>
<style scoped lang="scss">
.parallax {
  background-attachment: fixed;
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  background-image: url("public/medias/Screen-Shot-2022-11-15-at-1.11.12-PM-e1668540813864-1024x682.jpg");
  height: 50em;
}
.main {
  height: 100%;
  &__container {
    &__img {
      display: flex;
      object-fit: cover;
    }
    &__title {
      font-size: 8em;
      padding: 0.5em;
    }
    &__text {
      background-color: white;
      height: 100%;
      padding-left: 2em;
      padding-right: 2em;
      font-weight: 300;
      font-size: x-large;
    }
  }
}
</style>
<script></script>
