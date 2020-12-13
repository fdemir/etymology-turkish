<template>
  <div class="word-page">
    <div class="container">
      <section class="word-page__section">
        <alert-box>
          <h1 class="m-0">{{ name }}</h1>
        </alert-box>
      </section>

      <section class="word-page__section">
        <h3 class="mb-2">Kaynak</h3>
        <span>
          {{ source }}
        </span>
      </section>

      <section class="word-page__section">
        <h3 class="mb-2">Kökeni</h3>
        <span>
          Fransızca collage "yapıştırma" sözcüğünden alıntıdır. Fransızca sözcük
          Fransızca coller "yapıştırmak" fiilinden +age sonekiyle türetilmiştir.
          Bu sözcük Fransızca colle "tutkal" sözcüğünden türetilmiştir. Sözcük
          Latince aynı anlama gelen colla sözcüğünden evrilmiştir.
        </span>
      </section>

      <section class="word-page__section">
        <h3 class="mb-2">Ek Bilgi</h3>
        <span v-html="additional_desc"> </span>
      </section>
    </div>
  </div>
</template>

<script>
export default {
  async asyncData({ error, params, $axios }) {
    const { value } = params
    try {
      const result = await $axios.get('/word/' + value)
      const { value: name, additional_desc, source } = result.data
      return {
        name,
        additional_desc,
        source,
      }
    } catch {
      error({ statusCode: 404 })
    }
  },
  data() {
    return {
      name: '',
      additional_desc: '',
      source: '',
    }
  },
}
</script>

<style lang="scss" scoped>
.word-page {
  padding: 60px 0;

  &__section {
    margin-bottom: 25px;
  }
}
</style>
