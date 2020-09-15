<template>
  <div class="search-input">
    <div class="search-input-box">
      <i class="search-input-box__icon">
        <SearchIcon />
      </i>
      <input
        type="text"
        class="search-input-box__input"
        placeholder="bir kelime, sözcük"
      />
    </div>
    <button class="search-input-random-btn">
      <ShuffleIcon />
    </button>
  </div>
</template>

<script>
import SearchIcon from 'feather-icons/dist/icons/search.svg?inline'
import ShuffleIcon from 'feather-icons/dist/icons/shuffle.svg?inline'

export default {
  components: {
    SearchIcon,
    ShuffleIcon,
  },
}
</script>

<style lang="scss" scoped>
/* stylelint-disable */
$input-icon-width: 40px;
$input-height: 45px;

.search-input {
  display: flex;
  margin-bottom: 30px;

  &-box {
    width: 400px;
    height: $input-height;
    border-radius: 6px;
    background: #fff;
    border: 1px solid #434a54;
    box-shadow: 4px 3px 0px rgba(0, 0, 0, 0.25);
    margin-right: 25px;
    position: relative;
    padding-left: $input-icon-width;
    display: flex;

    &__icon {
      position: absolute;
      left: 0;
      top: 0;
      height: 100%;
      width: $input-icon-width;
      background: transparent;
      display: flex;
      justify-content: center;
      align-items: center;

      svg {
        width: 22px;
      }
    }

    &__input {
      flex: 1;
      outline: 0;
      padding: 0;
      border: 0;
      margin: 2px;

      &::placeholder {
        color: #4f4f4f;
      }
    }
  }

  &-random-btn {
    background: #ffffff;
    mix-blend-mode: normal;
    border: 1px solid #434a54;
    box-sizing: border-box;
    box-shadow: 4px 3px 0px rgba(0, 0, 0, 0.25);
    border-radius: 100%;
    height: $input-height;
    width: $input-height;
    cursor: pointer;

    svg {
      width: 22px;
    }
  }
}
</style>
