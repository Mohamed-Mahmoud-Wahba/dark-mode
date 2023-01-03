<template>
  <div
    class="col-lg-4 col-md-6 card"
    :style="isDarkMode ? { backgroundColor: 'black', color: 'white' } : null"
  >
    <img :src="card.img" alt="" />
    <div class="content">
      <h3 class="mt-4">{{ card.title }}</h3>
      <p>{{ card.author }}</p>
    </div>
  </div>
</template>
<script setup lang="ts">
interface CardProps {
  card: {
    img: string;
    title: string;
    author: string;
  };
}
const { isDarkMode } = useDarkMode();
const props = defineProps<CardProps>();
</script>

<style scoped>
.card {
  text-align: center;
  padding: 25px;
  max-width: 390px;
  margin: 15px;
}

img {
  width: 100%;
  height: 100%;
  max-height: 200px;
}

.content {
  padding: 10px;
}

p {
  margin-top: 10px;
}
</style>
