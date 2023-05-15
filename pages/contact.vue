<template>
  <main>
    <div class="main__container container">
      <H1 class="main__container__title"> Nous contacter</H1>
    </div>
    <div class="parallax">
      
    </div>
    <form>
      <div class="form-group">
        <label for="email">Email:</label>
        <input
          type="email"
          id="email"
          name="email"
          placeholder="Entrez votre adresse email"
        />
      </div>

      <div class="form-group">
        <label for="message">Message:</label>
        <textarea
          id="message"
          name="message"
          placeholder="Entrez votre message ici"
        ></textarea>
      </div>

      <button type="submit">Envoyer</button>
    </form>
  </main>
</template>
<style scoped lang="scss">
.parallax {
  background-attachment: fixed;
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  background-image: url("public/medias/Power-bandw.jpg");
  height: 50em;
}
.main {
  &__container {
    &__title {
      text-align: center;
      font-size: 10em;
    }
  }
  &__form {
    text-align: center;
  }
}
form {
  max-width: 600px;
  margin: 0 auto;
}

.form-group {
  display: flex;
  flex-direction: row;
  align-items: center;
  margin-bottom: 1em;
  margin-top: 3em;
}

label {
  margin-right: 0.5em;
  width: 5em;
  text-align: right;
  font-size: xx-large;
}

input,
textarea {
  width: 100%;
  padding: 0.5em;
  background-color: #eeb314;
  border: none;
  border-radius: 4px;
  padding-bottom: 4em;
}

button[type="submit"] {
  background-color: #cf7007;
  color: white;
  padding: 0.5em;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  margin-left: 10em;
}

button[type="submit"]:hover {
  background-color: #ff9000;
}
</style>
