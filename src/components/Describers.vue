<script setup></script>

<template>
  <div class="wrapper">
    <img src="@/assets/pfp.jpg" alt="Profile picture">

    <div class="name">

      <span class="main">Grigory <br> Vodyanov</span>

      <span class="sub">Григорий Водянов</span>

    </div>
  </div>
</template>

<style scoped>
.wrapper {
  flex-grow: 100;
  display: flex;
  flex-direction: row;
  justify-content: center;
  margin: 2rem 0.5rem;
  gap: 4rem;
  align-items: center;
  align-content: center;
  flex-wrap: wrap;
  height: 100%;
}

@media only screen and (min-width: 400px) {
  .wrapper {
    margin: 2rem 4rem;
  }
}

img {
  height: 15rem;
  width: 15rem;
  border-radius: 100%;
}

.name {
  display: flex;
  justify-content: flex-end;
  flex-direction: row;
  line-height: 5rem;
  flex-direction: column;
}

.main {
  font-size: 4rem;
  font-weight: 900;
}

.sub {
  color: var(--bg4);
  font-style: italic;
  font-size: 1.5rem;
}
</style>