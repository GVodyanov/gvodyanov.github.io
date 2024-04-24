<script setup>
import {
  RiGithubLine,
  RiDiscordLine,
  RiStackOverflowLine,
  RiMailLine,
  RiLeafLine,
  RiLinkedinLine,
  RiInstagramLine
} from '@remixicon/vue'
</script>

<template>
  <div class="contacts">
    <a href="https://github.com/GVodyanov" class="contact zoomable">
      <RiGithubLine size="3rem" color="#F5F5F5" className="my-icon" />
      GitHub
    </a>
    <a href="https://discordapp.com/users/620090816140148736" class="contact zoomable">
      <RiDiscordLine size="3rem" color="#F5F5F5" className="my-icon" />
      Discord
    </a>
    <a href="https://stackoverflow.com/users/17331482/scratchx" class="contact zoomable">
      <RiStackOverflowLine size="3rem" color="#F5F5F5" className="my-icon" />
      Stack Overflow
    </a>
    <a href="mailto:scratchx@gmx.com" class="contact zoomable">
      <RiMailLine size="3rem" color="#F5F5F5" className="my-icon" />
      Email
    </a>
    <a href="https://rosalind.info/users/Grigory_VV/" class="contact zoomable">
      <RiLeafLine size="3rem" color="#F5F5F5" className="my-icon" />
      Rosalind
    </a>
    <a href="https://www.linkedin.com/in/grigory-vodyanov-099505241/" class="contact zoomable">
      <RiLinkedinLine size="3rem" color="#F5F5F5" className="my-icon" />
      LinkedIn
    </a>
    <a href="https://www.instagram.com/grigory_vodyanov/" class="contact zoomable">
      <RiInstagramLine size="3rem" color="#F5F5F5" className="my-icon" />
      Instagram
    </a>
  </div>
</template>

<style scoped>
.contacts {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  align-content: center;
  gap: 1rem;
  padding: 2rem;
}

a {
  padding: 1.5rem;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px, rgba(0, 0, 0, 0.12) 0px -12px 30px,
    rgba(0, 0, 0, 0.12) 0px 4px 6px, rgba(0, 0, 0, 0.17) 0px 12px 13px,
    rgba(0, 0, 0, 0.09) 0px -3px 5px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  font-weight: bold;
  text-decoration: none;
  gap: 1rem;
  color: #f5f5f5;
  flex-grow: 0;
  flex-basis: 0;
  width: 10rem;
  background-color: #161617;
  text-align: center;
}

@media screen and (max-width: 1000px) {
  a {
    padding: 1rem;
    flex-basis: 7rem;
    height: 7rem;
  }

  .contacts {
    flex-direction: row;
    justify-content: center;
    flex-wrap: wrap;
  }
}
</style>
