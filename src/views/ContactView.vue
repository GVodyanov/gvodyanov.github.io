<script setup></script>

<template>
  <div class="contact-wrapper">
    <div class="contacts">
      <a href="https://github.com/ScratchX98" class="contact">
        <i class="nf nf-fa-github"></i>
        Github
      </a>
      <a href="https://reddit.com/u/scratchx98" class="contact">
        <i class="nf nf-fa-reddit"></i>
        Reddit
      </a>
      <a href="https://discordapp.com/users/620090816140148736" class="contact">
        <i class="nf nf-md-discord"></i>
        Discord
      </a>
      <a href="https://stackoverflow.com/users/17331482/scratchx" class="contact">
        <i class="nf nf-fa-stack_overflow"></i>
        Stack Overflow
      </a>
      <a href="mailto:scratchx@gmx.com" class="contact">
        <i class="nf nf-md-email"></i>
        Email
      </a>
      <a href="https://rosalind.info/users/Grigory_VV/" class="contact">
        <i class="nf nf-fae-dna"></i>
        Rosalind
      </a>
    </div>
  </div>
</template>

<style scoped>
.contacts {
  display: flex;
  flex-wrap: wrap;
  padding: 2rem;
  gap: 1rem;
  justify-content: start;
}


@media only screen and (min-height: 800px) {
  .about ul {
    gap: 3rem;
  }
}

.contact-wrapper {
  flex-grow: 100;
}

a {
  text-decoration: none;
  font-size: 1.5rem;
  color: var(--bg);
  padding: 1rem;
  border-radius: 1rem;
  background-color: var(--fg1);
}
</style>