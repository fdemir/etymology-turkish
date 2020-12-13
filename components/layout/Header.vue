<template>
  <div class="navbar">
    <div class="container navbar-container">
      <n-link to="/">
        <img src="~/assets/images/logo.svg" class="navbar-logo" alt="" />
      </n-link>
      <div>
        <ul class="navbar-links">
          <li>
            <n-link to="">Ana Sayfa</n-link>
          </li>
          <li>
            <n-link to="/bilgi">Bilgi</n-link>
          </li>
          <li>
            <n-link to="/">Rastgele</n-link>
          </li>
          <li>
            <a href="https://github.com/frndmr/etymology-turkish">Github</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
/* stylelint-disable */
@import '~/assets/scss/partials/breakpoints';

.navbar {
  height: 82px;
  width: 100%;
  background: transparent;
  z-index: 100;

  &-logo {
    height: 50px;
  }

  &-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100%;
  }

  &-links {
    display: flex;
    list-style-type: none;

    @include bp(tablet-sm) {
      display: none;
    }

    li {
      padding-left: 35px;
      display: flex;
      font-family: 'Roboto Mono';
      color: #4f4f4f;

      &.has-icon {
        font-size: 24px;
      }

      a {
        text-decoration: none;
        cursor: pointer;
        color: inherit;
      }
    }
  }
}
</style>
