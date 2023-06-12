<script setup></script>

<template>
  <ul class="project-wrapper">
    <li class="project">
      <a href="https://notes-lib.github.io">
        <i class="nf nf-md-book_arrow_right one"></i>
        <h2>Notes-lib</h2>
      </a>
      A website containing education articles submitted by the community. Built with Vue.js, PHP RESTful API, and MySQL.
    </li>
    <li class="project">
      <a href="https://github.com/ScratchX98/Mindrev">
        <i class="nf nf-md-book_arrow_right two"></i>
        <h2>Mindrev</h2>
      </a>
      An application for organizing notes and flashards to help you study. Built with Flutter.
    </li>
    <li class="project">
      <a href="https://github.com/FerMeLive">
        <i class="nf nf-md-book_arrow_right three"></i>
        <h2>FerMe</h2>
      </a>
      A social media with an app and website created with some friends. Built with vanilla JS, PHP RESTful API, Flutter,
      and MySQL.
    </li>
  </ul>
</template>

<style scoped>
@import "https://www.nerdfonts.com/assets/css/webfont.css";

.project-wrapper {
  display: flex;
  flex-grow: 100;
  flex-direction: column;
  padding: 2rem;
  gap: 1rem;
  list-style-type: none;
}

@media only screen and (min-height: 800px) {
  .about ul {
    gap: 3rem;
  }
}

.project {
  line-height: 2;
}

a {
  color: var(--bg);
  display: flex;
  align-items: center;
  align-content: center;
  text-decoration: none;
}

a i {
  text-decoration: none;
}

.one {
  color: var(--orange-dim);
}

.two {
  color: var(--green-dim);
}

.three {
  color: var(--yellow-dim);
}
</style>
