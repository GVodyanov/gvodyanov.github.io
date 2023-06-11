<script setup>
import Greetings from '@/components/Greetings.vue';
import Describers from '@/components/Describers.vue';

</script>

<template>
  <Greetings />
  <Describers />
</template>

<style scoped>
.main-wrapper {
  display: flex;
  flex-direction: column;
  justify-content: stretch;
  flex-grow: 1;
  height: 100%;
}
</style>
