<template>
  <div class="error-page">
    <h1>404 introuvable</h1>
    <img src="https://media1.giphy.com/media/IVDYYv6Cto6LS/giphy.webp" alt="" />
    <p>impossible de trouver la page essaie encore</p>
    <router-link to="/">retour a l'envoyeur</router-link>
  </div>
</template>

<style>
.error-page {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100%;
}

h1 {
  font-size: 5em;
  margin-bottom: 2rem;
}

p {
  font-size: 2em;
  margin-bottom: 2em;
}

router-link {
  font-size: 2em;
}
</style>
