<script setup>
const props = defineProps({
  name: String,
  image: String,
});

import { ref } from 'vue';
const likes = ref(0);

function handleLike() {
  likes.value++;
}
</script>

<template>
  <div class="gallery-label">
    <NuxtImg :src="image" :alt="name" loading="lazy" />
    <div class="img-caption">{{ name }}</div>
    <div class="like-button" @click="handleLike">
      <img src="/pics/thumbs-up.svg" alt="like" />
      <span class="like-count">{{ likes }}</span>
    </div>
  </div>
</template>

<style>
.gallery-label {
  position: relative;
  text-align: center;
  overflow: hidden;
  aspect-ratio: 4 / 3;
}

.gallery-label img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
  border-radius: 10px;
}

.gallery-label:hover {
  transform: scale(1.2);
  transition: 0.7s ease;
  z-index: 1;
  cursor: pointer;
}

.img-caption {
  padding: 0.4rem;
  color: white;
  text-align: center;
  background: transparent;
  position: absolute;
  left: 0;
  bottom: 0;
  width: calc(100% - 40px);
  text-overflow: ellipsis;
}

.like-button {
  display: flex;
  position: absolute;
  align-items: center;
  bottom: 4px;
  right: 4px;
  text-decoration: none;
  color: white;
  border-radius: 3px;
  gap: 4px;
}

.like-button:hover {
  background-color: rgb(46, 220, 46);
}

.like-button img {
  width: 20px;
  height: 20px;
  filter: invert(1);
}
</style>
