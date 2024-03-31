<script setup>
import { RouterView } from 'vue-router'
import NavBar from './components/NavBar.vue'
</script>

<template>
  <div class="backdrop">
    <div class="inner">
      <RouterView />
      <NavBar />
    </div>
  </div>
</template>

<style scoped>
.backdrop {
  height: 100%;
  width: 100%;
  display: flex;
  justify-content: center;
  align-content: center;
  align-items: center;
  background: url("./assets/back.jpg") bottom center no-repeat;
  background-size: cover;
}

.page {
  height: 100%;
  flex-grow: 1;
}

@media only screen and (min-height: 800px) {
  .inner {
    max-height: 40rem;
    max-width: 50rem;
  }
}

.inner {
  height: 100%;
  width: 100%;
  overflow: hidden;
  background-color: var(--fg);
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
    rgba(0, 0, 0, 0.12) 0px -12px 30px,
    rgba(0, 0, 0, 0.12) 0px 4px 6px,
    rgba(0, 0, 0, 0.17) 0px 12px 13px,
    rgba(0, 0, 0, 0.09) 0px -3px 5px;
  display: flex;
  flex-direction: column;
  justify-items: stretch;
}
</style>
