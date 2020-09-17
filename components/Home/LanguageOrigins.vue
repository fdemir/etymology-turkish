<template>
  <div class="language-origins">
    <h3>
      Köken Diller
      <link-button> > </link-button>
    </h3>
    <div class="language-origins__row">
      <language-card text="Türkçe" />
      <language-card text="Almanca" />
      <language-card text="İngilizce" />
      <language-card text="Kürtçe" />
    </div>
  </div>
</template>

<script>
import LanguageCard from '~/components/LanguageCard'
export default {
  components: {
    LanguageCard,
  },
}
</script>

<style lang="scss" scoped>
.language-origins {
  &__row {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 15px;
  }
}
</style>
