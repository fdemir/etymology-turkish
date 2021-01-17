<template>
  <div class="category-page">
    <div class="container">
      <div>
        <h1 class="mb-1">Eski Türkçe Bölümü</h1>
        <span
          >Deneme ile ilgili olan sözcüklerin kökenlerinin incelemeleri:</span
        >
      </div>
      <div class="category-page__list">
        <word-card v-for="x in 10" :key="x" />
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.category-page {
  padding: 60px 0;

  &__list {
    padding-top: 30px;
  }
}
</style>
