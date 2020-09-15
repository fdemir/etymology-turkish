<template>
  <div class="language-card">
    <Card> {{ text }} </Card>
  </div>
</template>

<script>
import { Card } from '~/components/ui'
export default {
  props: {
    text: {
      type: String,
      default: '',
    },
  },
  components: {
    Card,
  },
}
</script>

<style lang="scss">
.language-card .card {
  box-shadow: 0 5px 0 #2f80ed !important;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100px;
  cursor: pointer;
}
</style>
