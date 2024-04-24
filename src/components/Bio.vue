<script setup></script>

<template>
  <div class="bio">
    <article>
      <strong>Me:</strong>
      <br />
      <p class="zoomable">
        I am a scientific lyceum student of applied sciences with a passion for software development
        and engineering. Most of my experience comes from the development of ERP systems for local
        companies in northern Italy. I have also won a few academic awards and am a former school
        representative of my lyceum.
      </p>
    </article>
    <article>
      <strong>Languages:</strong>
      <br />
      <ul>
        <li class="zoomable">English</li>
        <li class="zoomable">Italian</li>
        <li class="zoomable">Russian</li>
      </ul>
    </article>
    <article>
      <strong>Currently learning:</strong>
      <br />
      <ul>
        <li class="zoomable">German</li>
        <li class="zoomable">Rust</li>
        <li class="zoomable">AI</li>
      </ul>
    </article>
    <article>
      <strong>Interests:</strong>
      <br />
      <p class="zoomable">
        Software development, applied physics, data analysis, philosophy, open source, sustainable
        urbanism, logistics, craft beer, woodworking, baking, SailGP, and much much more
      </p>
    </article>
  </div>
</template>

<style scoped>
.bio {
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

p {
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px, rgba(0, 0, 0, 0.12) 0px -12px 30px,
    rgba(0, 0, 0, 0.12) 0px 4px 6px, rgba(0, 0, 0, 0.17) 0px 12px 13px,
    rgba(0, 0, 0, 0.09) 0px -3px 5px;
  padding: 1rem;
  flex-grow: 20;
  display: flex;
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
  padding: 2rem;
  flex-grow: 1;
  text-align: center;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px, rgba(0, 0, 0, 0.12) 0px -12px 30px,
    rgba(0, 0, 0, 0.12) 0px 4px 6px, rgba(0, 0, 0, 0.17) 0px 12px 13px,
    rgba(0, 0, 0, 0.09) 0px -3px 5px;
  font-weight: bold;
}
</style>
