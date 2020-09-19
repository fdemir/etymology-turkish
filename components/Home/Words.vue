<template>
  <div class="words-section">
    <WordCategories />
    <DailyWord />
  </div>
</template>

<style lang="scss" scoped>
/* stylelint-disable */
@import '~/assets/scss/partials/breakpoints';

.words-section {
  display: grid;
  grid-template-columns: 6fr 5fr;
  grid-column-gap: 15px;

  @include bp(tablet-sm) {
    grid-template-columns: 1fr;
  }
}
</style>
