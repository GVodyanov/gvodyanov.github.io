<script setup>
import { RouterLink } from 'vue-router'

</script>

<template>
  <ul>
    <li>
      <RouterLink to="/">Home</RouterLink>
    </li>
    <li>
      <RouterLink to="/about">About</RouterLink>
    </li>
    <li>
      <RouterLink to="/projects">Projects</RouterLink>
    </li>
    <li>
      <RouterLink to="/contacts">Contacts</RouterLink>
    </li>

  </ul>
</template>

<style scoped>
ul {
  display: flex;
  justify-content: space-between;
  align-content: center;
  align-items: center;
  list-style-type: none;
  flex-direction: row;
  flex-shrink: 1;
  gap: 0.5rem;
  margin: 2rem 0.5rem;
}

@media only screen and (min-width: 400px) {
  ul {
    margin: 2rem 4rem;
  }
}

li a {
  color: var(--bg);
  text-decoration: none;
  text-transform: uppercase;
}
</style>
