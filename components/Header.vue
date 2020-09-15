<template>
  <div class="navbar">
    <div class="container navbar-container">
      <div>
        <img src="~/assets/images/elibelinde.png" style="height: 50px" alt="" />
      </div>
      <div>
        <ul class="navbar-links">
          <li>
            <n-link to="">Ana Sayfa</n-link>
          </li>
          <li>
            <n-link to="/random">Rastgele</n-link>
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
.navbar {
  height: 82px;
  width: 100%;
  background: #fff;
  border-bottom: 1px solid #eff0f0;
  z-index: 100;

  &-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100%;
  }

  &-links {
    display: flex;
    list-style-type: none;

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
