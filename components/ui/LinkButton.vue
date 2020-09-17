<template>
  <n-link to="/" class="link-button"><slot /></n-link>
</template>

<style lang="scss" scoped>
/* stylelint-disable */
.link-button {
  border-radius: 6px;
  background: rgba(47, 128, 237, 0.1);
  color: #2f80ed;
  padding: 4px 12px;
  text-decoration: none;
  font-family: 'Roboto Mono';
  font-weight: 500;
}
</style>
