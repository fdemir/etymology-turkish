<template>
  <div class="content">
    <SearchSection />
    <main class="container">
      <section>
        <Description />
      </section>
      <section>
        <LanguageOrigins />
      </section>
    </main>
  </div>
</template>

<script>
import SearchSection from '~/components/Home/SearchSection'
import Description from '~/components/Home/Description'
import LanguageOrigins from '~/components/Home/LanguageOrigins'

export default {
  components: {
    SearchSection,
    Description,
    LanguageOrigins,
  },
}
</script>

<style lang="scss" scoped>
.content {
  main {
    padding: 25px 0;

    section {
      padding-bottom: 30px;
    }
  }
}
</style>
