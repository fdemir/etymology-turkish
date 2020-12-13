<template>
  <div class="daily-word">
    <card>
      <h3 class="mt-0 mb-1 daily-word__title">Kolaj</h3>
      <div>
        <div class="mb-2">
          <i>1960 yılından önce</i>
        </div>
        <div>
          - <span class="font-weight-semibold">Fr</span> collage yapıştırma
          <span class="font-weight-semibold">Fr</span> coller yapıştırmak +age
          <span class="font-weight-semibold">Fr</span> colle tutkal Lat colla
          a.a.
        </div>
      </div>
    </card>
  </div>
</template>

<style lang="scss" scoped>
.daily-word {
  /* refactor */
  display: flex;
  flex-direction: column;
  flex: 1;

  .card {
    flex: 1;
  }

  &__title {
    background: #f2c94c;
    display: inline-block;
    padding: 2px;
    margin-bottom: 0.5rem;
  }
}
</style>
