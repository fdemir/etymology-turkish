<template>
  <div class="search-section">
    <div class="container">
      <h2>Bir kelime ara...</h2>
      <!-- <div class="search-section-input">
        <input type="text" placeholder="..." />
      </div> -->
    </div>
  </div>
</template>

<style lang="scss" scoped>
.search-section {
  height: 320px;
  width: 100%;
  background: #f1f3f8;
  display: flex;

  .container {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
  }

  &-input {
    input {
      width: 400px;
      border: 1px solid rgba(225, 225, 225, 0.76);
      background: #fff;
      padding: 1rem;
      border-radius: 6px;
    }
  }
}
</style>
