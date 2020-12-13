<template>
  <div class="search-section">
    <h1 class="search-section__title">Türkçe</h1>
    <SearchInput />
  </div>
</template>

<style lang="scss" scoped>
.search-section {
  height: 400px;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;

  &__title {
    color: #333;
    margin-bottom: 40px;
  }
}
</style>
