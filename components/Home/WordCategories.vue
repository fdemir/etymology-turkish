<template>
  <div class="word-categories">
    <h3>
      Kelime Kategorileri
      <link-button> > </link-button>
    </h3>
    <div class="word-categories-row">
      <card>
        <h3 class="mt-0 mb-1">Türeme</h3>
        <ul class="word-list mb-2">
          <li>kolaj</li>
          <li>enva</li>
          <li>seramik</li>
          <li>polarize</li>
        </ul>
        <link-button>Tümünü Göster ></link-button>
      </card>
      <card>
        <h3 class="mt-0 mb-1">Ses Evrimi</h3>
        <ul class="word-list mb-2">
          <li>pelikan</li>
          <li>orta</li>
          <li>bulamak</li>
          <li>çek</li>
        </ul>
        <link-button>Tümünü Göster ></link-button>
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
    grid-template-columns: repeat(2, 1fr);
    grid-column-gap: 15px;

    @include bp(mobile-sm) {
      grid-template-columns: 1fr;
      grid-row-gap: 15px;
    }
  }

  .word-list {
    display: flex;
    flex-direction: column;
    list-style: none;

    li {
      color: #4f4f4f;
      padding: 4px 0;
    }
  }
}
</style>
