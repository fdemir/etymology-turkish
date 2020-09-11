<template>
  <div class="navbar">
    <div class="container navbar-container">
      <div>
        <img src="~/assets/images/elibelinde.png" style="height: 70px" alt="" />
      </div>
      <div>
        <ul class="navbar-links">
          <li>
            <a href="https://github.com/frndmr/etymology-turkish">
              <ion-icon name="logo-github" />
            </a>
          </li>
          <li>
            <a href="">
              <ion-icon name="logo-twitter" />
            </a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.navbar {
  height: 82px;
  width: 100%;
  background: #fff;
  box-shadow: 0 5px 4px rgba(0, 0, 0, 0.04);

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
      padding-left: 20px;
      display: flex;
      font-size: 24px;

      a {
        color: inherit;
      }
    }
  }
}
</style>
