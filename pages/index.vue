<template>
  <div class="content">
    <SearchSection />
  </div>
</template>

<script>
import SearchSection from '~/components/Home/SearchSection'
export default {
  components: {
    SearchSection,
  },
}
</script>

<style lang="scss" scoped>
.content {
  min-height: 100vh;
}
</style>
