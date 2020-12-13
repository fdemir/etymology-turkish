<template>
  <div class="search-input">
    <div class="search-input-box">
      <i class="search-input-box__icon">
        <SearchIcon />
      </i>
      <input
        type="text"
        class="search-input-box__input"
        placeholder="sözcük arat"
      />
    </div>
    <!-- <button class="search-input-random-btn">
      <ShuffleIcon />
    </button> -->
  </div>
</template>

<script>
import SearchIcon from 'feather-icons/dist/icons/search.svg?inline'

export default {
  components: {
    SearchIcon,
  },
}
</script>

<style lang="scss" scoped>
/* stylelint-disable */
@import '~/assets/scss/partials/breakpoints';
$input-icon-width: 40px;
$input-height: 50px;

.search-input {
  display: flex;

  @include bp(mobile-sm) {
    &-random-btn {
      display: none;
    }
    &-box {
      margin: 0 !important;
    }
  }

  @include bp(tablet-sm) {
    width: 100%;

    &-box {
      width: auto !important;
      flex: 1;
    }
  }

  &-box {
    width: 450px;
    height: $input-height;
    background: #ffffff;
    mix-blend-mode: normal;
    box-shadow: 0px 100px 80px rgba(0, 0, 0, 0.07),
      0px 41.7776px 33.4221px rgba(0, 0, 0, 0.0372137),
      0px 22.3363px 17.869px rgba(0, 0, 0, 0.023046),
      0px 12.5216px 10.0172px rgba(0, 0, 0, 0.0143632),
      0px 6.6501px 5.32008px rgba(0, 0, 0, 0.00826158),
      0px 2.76726px 2.21381px rgba(0, 0, 0, 0.00364935);
    border-radius: 12px;
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
      background: transparent;

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
