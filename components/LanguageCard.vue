<template>
  <div class="language-card">
    <card> {{ text }} </card>
  </div>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      default: '',
    },
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
