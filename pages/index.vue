<template>
  <div class="content">
    <SearchSection />
    <main class="container">
      <section>
        <Description />
      </section>
      <section>
        <Words />
      </section>
      <section>
        <LanguageOrigins />
      </section>
    </main>
  </div>
</template>

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
