<template>
  <div class="word-categories">
    <div class="word-categories-row">
      <card v-for="x in 6" :key="x" class="word-categories-col">
        <h3 class="mt-0 mb-0">Türeme</h3>
        <ul class="word-list mb-2">
          <li>kolaj</li>
          <li>seramik</li>
          <li>polarize</li>
        </ul>
        <link-button>Tümünü Gör</link-button>
      </card>
    </div>
  </div>
</template>

<style lang="scss" scoped>
/* stylelint-disable */
@import '~/assets/scss/partials/breakpoints';

.word-categories {
  &-row {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;

    @include bp(mobile-sm) {
      grid-template-columns: 1fr;
    }
  }

  &-col {
    margin-bottom: 30px;
  }

  .word-list {
    display: flex;
    flex-direction: column;
    list-style: none;

    li {
      color: #4f4f4f;
      padding: 4px 0;
      cursor: pointer;
      font-family: 'Roboto Mono';

      &::before {
        content: '-';
        margin-right: 10px;
      }
    }
  }
}
</style>
