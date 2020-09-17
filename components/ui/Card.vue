<template>
  <div class="card">
    <slot />
  </div>
</template>

<style lang="scss" scoped>
/* stylelint-disable */

.card {
  border: 0.5px solid #000;
  box-sizing: border-box;
  box-shadow: 0px 5px 0px rgba(0, 0, 0, 0.05);
  border-radius: 6px;
  padding: 1.3rem 1.5rem;
}
</style>
