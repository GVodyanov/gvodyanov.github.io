<template>
  <div class="about">
    <div class="about-wrapper">
      <ul>
        <li class="one"> <i class="nf nf-oct-location"></i> Padua, Italy</li>
        <li class="two"> <i class="nf nf-md-translate"></i> English, Russian, Italian </li>
        <li class="three"> <i class="nf nf-cod-book"></i> Scientific Lyceum "E. Fermi" of Padua, school representative
        </li>
        <li class="four"> <i class="nf nf-cod-code"></i> <span class="underline">Dart, PHP, Javascript</span>, SQL,
          Python,
          C++ </li>
        <li class="five"> <i class="nf nf-fa-gears"></i> Flutter, Vue.js </li>
        <li class="six"> <i class="nf nf-md-book_clock"></i> Learning Rust, Symfony, R </li>
      </ul>

      <hr>


      <p>I'm a student of applied sciences at the scientific lyceum <em>E. Fermi</em> of Padua with interests in physics,
        computer science, and biotech. Also known as ScratchX98.</p>
    </div>
  </div>
</template>

<style>
@import "https://www.nerdfonts.com/assets/css/webfont.css";

.about {
  padding: 2rem;
  flex-grow: 100;
  display: flex;
  justify-content: stretch;
}

.about-wrapper {
  display: flex;
  flex-direction: column;
  gap: 2rem;
  align-items: stretch;
  align-content: stretch;
  height: 100%;
}

.underline {
  text-decoration: underline;
}

.about ul {
  flex-grow: 1;
  display: flex;
  flex-direction: column;
  gap: 3rem;
  list-style-type: none;
  justify-content: space-between;
  height: 100%;
}

p {
  flex-grow: 1;
  flex-basis: 50%;
}

i {
  margin-right: 0.5rem;
}

.one i {
  color: var(--orange-dim);
}

.two i {
  color: var(--green-dim);
}

.three i {
  color: var(--yellow-dim);
}

.four i {
  color: var(--blue-dim);
}

.five i {
  color: var(--purple-dim);
}

.six i {
  color: var(--aqua-dim)
}
</style>
