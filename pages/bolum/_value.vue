<template>
  <div class="category-page">
    <div class="container">
      <div>
        <h1 class="mb-1">Eski Türkçe Bölümü</h1>
        <span
          >{{ title }} ile ilgili olan sözcüklerin kökenlerinin
          incelemeleri:</span
        >
      </div>
      <div class="category-page__list">
        <word-card v-for="x in 10" :key="x" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  async asyncData({ params, error, $axios }) {
    const { value } = params
    try {
      const result = await $axios.get('/category/' + value)
      return {
        title: result.data.name,
      }
    } catch {
      error({ message: 'Aradığınız bölüm bulunamadı.', statusCode: 404 })
    }
  },
  data() {
    return {
      title: 'Kategori',
    }
  },
  head() {
    return {
      title: this.title,
    }
  },
}
</script>

<style lang="scss" scoped>
.category-page {
  padding: 60px 0;

  &__list {
    padding-top: 30px;
  }
}
</style>
