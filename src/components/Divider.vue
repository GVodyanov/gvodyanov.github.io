<script setup>
//declare image string prop
const props = defineProps({
  image: String,
  offset: Number
})

const imageString = '/img/' + props.image + '.jpg'
const style = 'object-position: ' + props.offset
</script>

<template>
  <img :src="imageString" :alt="props.image" :style="style" />
</template>

<style scoped>
img {
  overflow: hidden;
  width: 1rem;
  object-fit: cover;
}

@media screen and (max-width: 1000px) {
  img {
    width: auto;
    min-height: 50px;
  }
}
</style>
