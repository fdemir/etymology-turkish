<template>
  <div class="content">
    <SearchSection />
    <main class="container">
      <section class="description">
        <Description />
      </section>
      <section class="words">
        <Words />
      </section>
      <section class="language-origins">
        <LanguageOrigins />
      </section>
    </main>
  </div>
</template>

<style lang="scss" scoped>
/* stylelint-disable */
@import '~/assets/scss/partials/breakpoints';

.content {
  main {
    padding: 25px 15px;
    display: flex;
    flex-direction: column;

    @include bp(tablet-sm) {
      padding-top: 0;

      section.description {
        order: 3;
      }
    }

    section {
      padding-bottom: 30px;
    }
  }
}
</style>
