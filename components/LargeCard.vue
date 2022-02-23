<template>
  <NuxtLink :to="`/products/${card.id}`" class="card">
    <img
      class="image"
      :src="require(`@/assets/images/${card.image || 'fe1.jpg'}`)"
      alt=""
    />
    <h3 class="header">{{ card.title }}</h3>
    <a class="snippet">
      {{ card.snippet }}
    </a>
  </NuxtLink>
</template>

<script>
export default {
  props: ["card"]
};
</script>

<style scoped>
.card {
  width: 31.5%;
  height: 25rem;
  border: none;
  overflow: hidden;
  padding: 0;
  cursor: pointer;
}
.image {
  height: 65%;
  border-radius: 0.5rem;
}
.header {
  font-size: 1.15rem;
  margin-top: 0.4rem;
  color: black;
  text-decoration: none !important;
}
.header:hover {
  text-decoration: none !important;
}
.snippet {
  color: grey;
}
a:hover {
  text-decoration: none;
  color: red;
}
</style>
