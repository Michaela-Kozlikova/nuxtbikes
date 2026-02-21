<script setup>
defineProps({
  title: String,
  image: String,
  description: String,
  specs: Array,
  brandColor: String
});
</script>

<template>
  <div class="main-content">
    <div class="bike-card">
      <img :src="image" :alt="title" width="600" height="auto" />
      <div class="list-items">
        <ul :style="{ '--dot-color': brandColor }">
          <li v-for="spec in specs" :key="spec">{{ spec }}</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped>
.bike-card {
  display: flex;
  padding: 40px;
  align-items: center;
  line-height: 30px;
  gap: 80px;
}

.bike-card img {
    border-radius: 10px;
    object-fit: cover;
    object-position: center;
    width: 600px;
    height: 430px;
}

.list-items li {
    font-size: 1rem;
}

.list-items ul {
    list-style-type: disc;
}

.list-items li::marker {
    font-size: 1.6rem;
    color: var(--dot-color, white);
}
</style>
