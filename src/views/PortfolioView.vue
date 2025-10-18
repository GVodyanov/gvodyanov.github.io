<template>
  <div class="background">
    <div class="portfolio-wrapper">
      <h1 class="portfolio-title">Portfolio - Grigory Vodyanov</h1>
      <div class="portfolio-intro">
        Hey! I am Grigory Vodyanov, welcome to my porfolio.
        <br /><br />
        I am a student at the Polytechnic University of Milan (the best technical university in
        Southern Europe), a Software Engineer at Nextcloud, and Co-Founder of the Public transport
        app PadoVia.it.
        <br /><br />
        My main passion is data: data protection, open data, digital sovereignty, and data
        engineering.
        <br /><br />
        Most of my experience comes from the development of Enterprise software focused on Data
        Protection and Open Source solutions. Here are some of the project I worked on recently:
        <br><br>
        <span class="grey">Please also check out <a href="https://github.com/GVodyanov">My Github</a>, I have a lot of work on there</span>
      </div>
      <div class="portfolio-list">
        <div class="portfolio-item" v-for="project in projects" :key="project.title">
          <!-- Render video embed HTML when present, otherwise render image only if defined -->
          <div v-if="project.video" class="portfolio-media" v-html="project.video"></div>
          <img v-else-if="project.image" :src="project.image" :alt="project.title" class="portfolio-image" />
          <div class="portfolio-info">
            <h2 class="project-title">{{ project.title }}</h2>
            <span class="project-desc">{{ project.description }}</span>
            <a :href="project.link" target="_blank" rel="noopener" class="project-link"
              >View Project</a
            >
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const projects = [
  {
    title: 'Nextcloud Groupware: Calendar, Contacts, Mail',
    link: 'https://github.com/nextcloud/calendar',
    image: '/img/calendar_application.png',
    description:
      'As part of my work for Nextcloud, I contributed heavily to the development of the Nextcloud Groupware apps, focusing mostly on the front-end in Vue.js and Pinia.'
  },
  {
    title: 'PadoVia.it - Public Transport App for Padua',
    link: 'https://padovia.it',
    image: '/img/padovia.png',
    description: 'I co-founded the PadoVia application for real time predictions and monitoring of public transport in Padua, with over 4000 daily users, featured on 6 different media outlets, including "Il Corriere della Sera". Built with React Native, Node.js, Redis, Clickhouse, and PostgreSQL.',
  },
  {
    title: 'IntraVia AI - AI Agent for Public Transport (work in progress)',
    link: 'https://www.intravia.it/en/ai',
    image: '/img/intravia.png',
    description: 'An LLM workflow based Agent that helps users plan trips using public transport in Italy, built with LlamaIndex, Qdrant, and the Open AI platform.',
  },
  {
    title: 'AI Detour Analyzer for updating GTFS Transport data',
    link: 'https://github.com/PadoVia/GTFSFixerAI',
    image: '/img/fixer.png',
    description: 'An AI-powered tool to automatically analyze detour announcements from public transport operators and update GTFS Transport data accordingly, built with LlamaIndex, Qdrant, and the Open AI platform.',
  },
  {
    title: 'AI Plant growth simulator',
    link: 'https://hackathon.bz.it/project/-project-genesis-',
    video: '<div style="padding:62.55% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/1106706455?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share" referrerpolicy="strict-origin-when-cross-origin" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="final"></iframe></div>',
    description: 'An AI-powered simulation engine that forecasts plant growth under given environmental conditions. Given an initial plant image and a set of stimuli, Project Genesis generates a new, photorealistic image of the plant\'s final state, along with a scientific description of what happened and why. Built for the NOI Summer Hackathon 2025. I contributed to the RAG and LLM integrations built with Llamaindex and Qdrant. I also created the front-end in Vue.js and the backend in Node.js.',
  },
  {
    title: 'H-orizon Agriculture Data Platform',
    link: 'https://github.com/GVodyanov/h-orizon',
    image: '/img/h-orizon.png',
    description: 'A webapp made for the NASA Space Apps Challenge 2024 hackathon, it helps farmers see the impact of climate change and weather patterns on their fields and suggestions crops to plant. Built with Vue.js and various geospatial data APIs.'
  },
  {
    title: 'Mindrev Study App',
    link: 'https://github.com/GVodyanov/Mindrev',
    image: '/img/mindrev.png',
    description:
      'An app for studying with flashcards, notes, and quizes built with Flutter.'
  }
]
</script>

<style scoped>
h1 {
  font-size: 2rem !important;
  /* slightly stronger text shadow for more depth */
  text-shadow: rgba(0, 0, 0, 0.12) 0 3px 2px, rgba(0, 0, 0, 0.12) 0 6px 4px,
    rgba(0, 0, 0, 0.12) 0 12px 8px, rgba(0, 0, 0, 0.12) 0 24px 16px;
}
.grey {
  font-style: italic;
  opacity: 0.8;
}
.background {
  background: #171718;
}
.portfolio-wrapper {
  max-width: 65rem;
  margin: 0 auto;
  padding: 2rem;
  display: flex;
  flex-direction: column;
  gap: 2rem;
  background: #171718;
  min-height: 100vh;
}
.portfolio-title {
  font-family: Molend, sans-serif;
  font-size: 2.8rem;
  margin-bottom: 1rem;
  color: #d7d7d7;
  text-align: center;
  padding: 1rem;
  /* stronger outer shadow + slightly stronger inset for more presence */
}
.portfolio-intro {
  font-size: 1.1rem;
  margin-bottom: 2rem;
  color: #bdbdbd;
}
.portfolio-list {
  width: 100%;
  display: flex;
  flex-direction: column;
  gap: 2rem;
}
.portfolio-item {
  background: #171718;
  /* stronger inset + more pronounced outer shadow */
  box-shadow: rgba(0, 0, 0, 0.4) 0 4px 12px;
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  gap: 1.5rem;
  padding: 2rem;
  transition: background 0.3s;
}
.portfolio-image {
  /* responsive image: prefer a percentage-based flex-basis, keep max width */
  flex: 0 0 55%;
  max-width: 600px;
  object-fit: contain;
  max-height: 30rem;
}

.portfolio-media {
  flex: 0 0 55%;
  max-width: 600px;
  width: 100%;
}

.portfolio-info {
  flex: 1 1 40%;
  min-width: 220px;
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}
.project-title {
  font-size: 1.5rem;
  color: #eaeaea;
  margin: 0;
}
.project-desc {
  color: #cfcfcf;
  margin: 0.5rem 0 0.75rem 0;
  line-height: 1.4;
  font-size: 0.98rem;
}
.project-link {
  color: #7fc7ff;
  text-decoration: underline;
  font-size: 1.1rem;
  word-break: break-all;
}
@media (max-width: 900px) {
  .portfolio-image {
    flex: 0 0 60%;
    width: 60vw;
    max-width: 100%;
    height: auto;
  }
}
@media (max-width: 600px) {
  .portfolio-item {
    flex-direction: column;
    align-items: flex-start;
    padding: 1rem;
  }
  .portfolio-image {
    flex: 0 0 100%;
    width: 100%;
    max-width: 100%;
    margin: 0 0 0.7rem 0;
    height: auto;
  }
  .portfolio-info {
    width: 100%;
    align-items: flex-start;
  }
}
</style>
