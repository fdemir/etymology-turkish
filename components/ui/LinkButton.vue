<template>
  <n-link to="/" class="link-button"><slot /></n-link>
</template>

<style lang="scss" scoped>
/* stylelint-disable */
.link-button {
  border-radius: 6px;
  background: #f3f3f3;
  color: #4f4f4f;
  padding: 4px 12px;
  text-decoration: none;
  font-family: 'Roboto Mono';
  font-weight: 500;

  &:hover {
    color: #fff;
    background: #4f4f4f;
  }
}
</style>
