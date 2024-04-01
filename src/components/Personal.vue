<script setup></script>

<template>
  <div class="personal">
    <img src="/pfp_cropped.jpg" alt="Grigory Vodyanov" />

    <h1>Grigory<br />Vodyanov</h1>

    <h3>Student at Scientific Lyceum "E. Fermi" of Padua, Software Engineer at Nextcloud</h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 900;
  color: #f5f5f5;
  background: -webkit-linear-gradient(white, #757575);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  text-shadow: rgba(0, 0, 0, 0.09) 0px 2px 1px, rgba(0, 0, 0, 0.09) 0px 4px 2px,
    rgba(0, 0, 0, 0.09) 0px 8px 4px, rgba(0, 0, 0, 0.09) 0px 16px 8px,
    rgba(0, 0, 0, 0.09) 0px 32px 16px;
  text-align: center;
  word-wrap: break-word;
  font-size: 400%;
}

h3 {
  margin-top: -1rem;
  font-weight: normal;
  margin-bottom: 2rem;
}

.personal {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  align-content: center;
  color: #75757aff;
  height: 100%;
  padding: 0rem 2rem;
  gap: 2rem;
  width: 100%;
}

img {
  margin-top: 2rem;
  filter: grayscale(100%);
  width: 15rem;
  margin-bottom: 1rem;
  box-shadow: rgba(240, 46, 170, 0.4) -5px 5px, rgba(240, 46, 170, 0.3) -10px 10px,
    rgba(240, 46, 170, 0.2) -15px 15px, rgba(240, 46, 170, 0.1) -20px 20px,
    rgba(240, 46, 170, 0.05) -25px 25px;
}

@media screen and (max-width: 2000px) {
  h1 {
    font-size: 250%;
  }

  .personal {
    padding: 0rem 1rem;
  }
}

@media screen and (max-width: 1500px) {
  h1 {
    font-size: 150%;
  }

  img {
    width: 8rem;
  }
}

@media screen and (max-width: 1000px) {
  h1 {
    font-size: 280%;
  }

  img {
    width: 15rem;
  }

  .personal {
    padding: 0rem 2rem;
  }
}
</style>
