<script setup>
import Personal from '@/components/Personal.vue'
import Bio from '@/components/Bio.vue'
import Experiences from '@/components/Experiences.vue'
import Contact from '@/components/Contact.vue'
import Divider from '@/components/Divider.vue'
</script>

<template>
  <div class="main-wrapper">
    <section class="first">
      <Personal />
    </section>
    <Divider image="moss" offset="left" />
    <section class="second">
      <Bio />
    </section>
    <Divider image="moss" offset="right" />
    <section class="third">
      <Experiences />
    </section>
    <Divider image="moss" offset="center" />
    <section class="last">
      <Contact />
    </section>
  </div>
</template>

<style scoped>
.main-wrapper {
  display: flex;
  flex-direction: row;
  justify-content: stretch;
  flex-grow: 1;
  height: 100vh;
  position: relative;
}

section {
  flex-grow: 50;
  flex-basis: 0;
  background-color: #101011;
  display: flex;
  height: 100%;
  overflow-y: auto;
  scrollbar-width: none; /* Firefox */
}

.second {
  flex-grow: 50;
}

.third {
  flex-grow: 60;
}

.last {
  flex-grow: 18;
  flex-shrink: 1;
  min-width: 17rem;
}

.first {
  flex-grow: 35;
}

section::-webkit-scrollbar {
  display: none;
}

img {
  flex-grow: 1;
}

@media screen and (max-width: 1000px) {
  .main-wrapper {
    flex-direction: column;
  }

  section {
    overflow-y: visible;
    height: auto;
  }
}
</style>
