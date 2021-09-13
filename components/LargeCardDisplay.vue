<template>
  <div class="container">
    <h4 class="header">Hello World</h4>
    <p class="snippet">Lorem ipsum dolor sit</p>
    <div class="card-container"></div>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style scoped>
  .container {
    margin-top: 2rem;
}
    .header {
        font-weight: 700;
        font-size: 1.5rem;
    }
    .snippet {
        color: grey;
        margin-bottom: 1.5rem;
    }
    .cards-container {
        display: flex;
        justify-content: space-between;
    }
</style>