<script setup></script>

<template>
  <div class="experiences">
    <article>
      <strong>I have experience in:</strong>
      <br />
      <ul>
        <li>
          <span>Vue.js</span>
          <p>
            I worked with Vue.js at two companies and have completed a few personal projects with
            it.
          </p>
        </li>
        <li>
          <span>Flutter and Dart</span>
          <p>
            I have developed a few apps with Flutter, some of which commercially at an internship.
          </p>
        </li>
        <li>
          <span>PHP</span>
          <p>
            I have made PHP APIs and worked on backends for ERP, CRM, and Collaboration systems,
            along with their respective databases.
          </p>
        </li>
        <li>
          <span>Linux system administration</span>
          <p>I have experience in setting up web serves and desktop linux system configuration.</p>
        </li>
      </ul>
    </article>
    <article>
      <strong>Achievements:</strong>
      <br />
      <ul>
        <li>
          <span>Second place in Italy in experimental physics</span>
          <p>Given by the EOES (European olympiads of experimental sciences) in 2023</p>
        </li>
        <li>
          <span>First place award at city science fair</span>
          <p>Given by "Sperimentando" of Padua in 2023</p>
        </li>
        <li>
          <span>Elected school representative of "E. Fermi" Lyceum</span>
          <p>2023/2024 school year</p>
        </li>
      </ul>
    </article>
    <article>
      <strong>Projects:</strong>
      <br />
      <ul>
        <li>
          <a href="https://notes-lib.github.io">Notes Library</a>
          <p>
            A website containing education articles submitted by the community. Built with Vue.js,
            PHP RESTful API, and MySQL.
          </p>
        </li>
        <li>
          <a href="https://github.com/ScratchX98/Mindrev">Mindrev</a>
          <p>
            An application for organizing notes and flashards to help you study. Built with Flutter.
          </p>
        </li>
        <li>
          <a href="https://github.com/FerMeLive">FerMe</a>
          <p>
            A social media with an app and website created with some friends. Built with vanilla JS,
            PHP RESTful API, Flutter, and MySQL.
          </p>
        </li>
      </ul>
    </article>
  </div>
</template>

<style scoped>
.experiences {
  display: flex;
  flex-direction: column;
  padding: 2rem;
  gap: 2rem;
  flex-grow: 1;
}

article {
  background-color: #171718;
  padding: 1rem;
  display: flex;
  flex-grow: 1;
  flex-basis: 0px;
  /*border-bottom: #75757a 0.2rem solid;
  border-right: #75757a 0.2rem solid;*/
  box-shadow: rgba(0, 0, 0, 0.06) 0px 2px 4px 0px inset;

  flex-direction: column;
  justify-content: center;
}

ul {
  list-style-type: none;
  padding: 0;
  display: flex;
  flex-direction: row;
  flex-grow: 20;
  align-content: center;
  align-items: center;
  gap: 2rem;
  flex-wrap: wrap;
}

li {
  flex-basis: 0;
  padding: 2rem;
  flex-grow: 1;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px, rgba(0, 0, 0, 0.12) 0px -12px 30px,
    rgba(0, 0, 0, 0.12) 0px 4px 6px, rgba(0, 0, 0, 0.17) 0px 12px 13px,
    rgba(0, 0, 0, 0.09) 0px -3px 5px;
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
  align-self: stretch;
}

li span,
a {
  font-weight: bold;
  color: #f5f5f5;
  text-decoration: none;
}
</style>
