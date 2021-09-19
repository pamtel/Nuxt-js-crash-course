<template>
  <div>
    <Nav />
    <div>
      <Hero />
      <div class="container">
        <LargeCardDisplay
          v-for="cardInfo in largeCardInfo"
          :key="cardInfo.id"
          :cardsSection="cardInfo"
        />
        <SmallCardDisplay
          v-for="cardInfo in smallCardInfo"
          :key="cardInfo.id"
          :cardsSection="cardInfo"
        />
      </div>
    </div>
  </div>
</template>

<script>
import { largeCardSections, smallCardSections  } from "@/assets/data.js";

export default {
  data() {
    return {
      largeCardInfo: largeCardSections,
      smallCardInfo: smallCardSections
    };
  }
};
</script>

<style scoped></style>
