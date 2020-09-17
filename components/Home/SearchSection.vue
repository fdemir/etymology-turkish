<template>
  <div class="search-section">
    <div class="search-section-body">
      <div class="search-section-body__container container">
        <h1 class="search-section-body__title">Kelime ara ✍️</h1>
        <SearchInput />
        <!-- refactor -->
        <div style="letter-spacing: 3px">Ç Ğ Ö Ş Ü</div>
      </div>
    </div>
  </div>
</template>

<script>
import SearchInput from './SearchInput'
export default {
  components: {
    SearchInput,
  },
}
</script>

<style lang="scss" scoped>
.search-section {
  padding: 18px;

  &-body {
    width: 100%;
    height: 300px;
    background: linear-gradient(
      180deg,
      rgba(51, 51, 51, 0.05) 0%,
      rgba(0, 0, 0, 0) 100%
    );
    border-radius: 6px;

    &__container {
      height: 100%;
      display: flex;
      justify-content: center;
      align-items: flex-start;
      flex-direction: column;
    }

    &__title {
      margin-bottom: 25px;
    }
  }
}
</style>
