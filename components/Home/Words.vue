<template>
  <div class="words-section">
    <WordCategories />
    <DailyWord />
  </div>
</template>

<style lang="scss" scoped>
.words-section {
  display: grid;
  grid-template-columns: 6fr 5fr;
  grid-column-gap: 15px;
}
</style>
