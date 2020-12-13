<template>
  <div class="words-section">
    <div class="words-section__desc">
      <h2 class="m-0">Sözcük Bölümleri</h2>
      <p>
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dignissimos
        libero nobis, nisi assumenda quibusdam rem fugit quidem aliquid qui vel
        officia reprehenderit voluptate alias natus maiores doloremque dolorem
        impedit dolores!
      </p>
    </div>
    <WordCategories />
    <!-- <DailyWord /> -->
  </div>
</template>

<style lang="scss" scoped>
/* stylelint-disable */
@import '~/assets/scss/partials/breakpoints';

.words-section {
  display: grid;
  grid-template-columns: 1fr;
  grid-column-gap: 15px;

  &__desc {
    padding-bottom: 40px;

    p {
      line-height: 24px;
    }
  }

  @include bp(tablet-sm) {
    grid-template-columns: 1fr;
  }
}
</style>
