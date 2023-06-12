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
  flex-basis: 2rem;
  display: flex;
  flex-direction: row;
  justify-content: center;
  margin: 2rem 0.5rem;
  gap: 2rem;
  align-items: center;
  align-content: center;
  flex-wrap: wrap;
  height: 100%;
}

.main {
  font-size: 3rem;
  font-weight: 900;
}

img {
  height: 10rem;
  width: 10rem;
  border-radius: 100%;
}

@media only screen and (min-width: 600px) {
  .main {
    font-size: 4rem;
  }

  img {
    height: 15rem;
    width: 15rem;
  }
}

.name {
  display: flex;
  justify-content: flex-end;
  flex-direction: row;
  line-height: 5rem;
  flex-direction: column;
}

.sub {
  color: var(--bg4);
  font-style: italic;
  font-size: 1.5rem;
}
</style>