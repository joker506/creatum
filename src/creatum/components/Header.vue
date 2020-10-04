<template>
  <div class="header">
    <div class="header__wrapp">
      <!-- <h1 class="header__title visully-hidden">Creatum</h1> -->

      <span class="header__logo--wrapp">
        <a href="#">
          <img src="~@/assets/Logo.svg" alt="header__logo" />
        </a>
      </span>
      <p
        @click="openMenu = !openMenu"
        v-bind:class="{ openmen: openMenu }"
        class="header__menu"
      >
        Menu
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      openMenu: false
    };
  },
  props: {
    msg: String
  }
};
</script>

<style lang="scss" scoped>
.header {
  //background-color: #fcfbf7;
}
.header__wrapp {
  margin: 0 auto;
  //background-color: aqua;
  max-width: 1200px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.header__menu {
  position: relative;
  padding-right: 40px;
  font-family: Montserrat, sans-serif;
  font-size: 18px;
  line-height: 100%;
  cursor: pointer;
  &::before {
    content: "";
    position: absolute;
    right: 0px;
    top: 3px;
    border: 2px solid #272727;
    width: 30px;
  }
  &::after {
    content: "";
    position: absolute;
    right: 12px;
    bottom: 3px;
    border: 2px solid #272727;
    width: 18px;
  }
}
.openmen {
  position: relative;

  &::before {
    top: -6px;
    right: 20px;
    height: 30px;
    width: 2px;
    border: none;
    // transition-delay: 0.2s;
    background-color: #272727;
    transform: rotate(45deg);
  }
  &::after {
    top: -6px;
    right: 20px;
    height: 30px;
    width: 2px;
    border: none;
    //transition: 0.2s;
    //transition-delay: 0.3s;
    background-color: #272727;
    transform: rotate(-45deg);
  }
}
</style>
