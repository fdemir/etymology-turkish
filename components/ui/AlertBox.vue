<template>
  <div class="alert-box">
    <div>
      <slot />
    </div>
  </div>
</template>

<style lang="scss" scoped>
.alert-box {
  display: flex;

  &::before {
    height: auto;
    width: 6px;
    border-radius: 4px;
    content: '';
    background: rgba(191, 158, 56, 0.5);
    margin-right: 20px;
  }
}
</style>
