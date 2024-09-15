<template>
  <div class="comic-card">
    <img :src="thumb" :alt="series" class="comic-thumb" />
    <div class="comic-details">
      <h3 class="comic-series">{{ series }}</h3>
      <p class="comic-price">{{ price }}</p>
      <span class="comic-type">{{ type }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ComicCard',
  props: {
    thumb: String,
    price: String,
    series: String,
    type: String
  }
}
</script>

<style lang="scss" scoped>
.comic-card {
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 8px;
  overflow: hidden;
  width: 200px;
  text-align: center;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  margin: 1rem;
  transition: transform 0.3s;

  &:hover {
    transform: scale(1.05);
  }

  .comic-thumb {
    width: 100%;
    height: auto;
  }

  .comic-details {
    padding: 1rem;

    .comic-series {
      font-size: 1.2rem;
      margin: 0.5rem 0;
      color: #333;
    }

    .comic-price {
      color: #555;
      font-weight: bold;
    }

    .comic-type {
      display: block;
      margin-top: 0.5rem;
      font-size: 0.9rem;
      color: #777;
    }
  }
}
</style>
