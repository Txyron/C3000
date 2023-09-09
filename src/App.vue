<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>

    <div class="wrapper">
      <img src="../src/assets/img/Logo1.png" alt="">
      <HelloWorld msg="Avis de passage" />

      <nav>
        <RouterLink to="/">Accueil</RouterLink>
        <RouterLink to="/about">Avis de passage</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
body{
  background: black;
}

header {
  line-height: 1.5;
  max-height: 100vh;
}


nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
}

nav a.router-link-exact-active {
  color: var(--color-text);
  color: aliceblue;

}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  margin: 5px;
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
  color: gray;
  text-decoration: none;
  border-radius: 3px;
  background: black;
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;
    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
