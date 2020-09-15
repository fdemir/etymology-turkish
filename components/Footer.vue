<template>
  <div class="footer">
    <div class="container footer-container">
      <div>
        <ul class="footer-links">
          <li>Hakkında</li>
          <li>Github</li>
          <li>TDK</li>
        </ul>
      </div>
      <div>
        <span>Copyright 2020 - Etimoloji</span>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.footer {
  width: 100%;
  height: 80px;
  .footer-container {
    display: flex;
    justify-content: space-between;
  }

  .footer-links {
    display: flex;
    list-style: none;
    margin: 0;
    padding: 0;

    li {
      padding-right: 30px;
    }
  }
}
</style>
