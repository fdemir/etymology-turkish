<template>
  <div class="content">
    <main class="container">
      <section class="description">
        <Description />
      </section>
      <section class="motifs-divider">
        <img src="~/assets/images/motifs-divider.png" width="100%" alt="" />
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
  background: url('~assets/images/elibelinde_transparent.png');
  background-repeat: no-repeat;
  background-position: 100% 50px;
  background-size: 300px, 150px;

  main {
    padding: 60px 15px;
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

      &.motifs-divider {
        padding: 30px 0;
      }
    }
  }
}
</style>
