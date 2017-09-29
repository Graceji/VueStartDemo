<template>
  <div class="header">
    <i @click="showAsideMenu" class="icon-menu"></i>
    <h1>My Bolg</h1>
  </div>
</template>

<script>
export default {
  methods: {
    showAsideMenu () {
      console.log(123)
    }
  }
}
</script>

<style lang="scss" scoped>
.header {
  display: flex;
  // flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 70px;
  background-color: #2196F3;
  color: #fff;

  i {
    width: 25px;
    height: 25px;
    display: inline-block;
    position: absolute;
    z-index: 1;
    flex: 1;
  }
  .icon-menu {
    background: url('../common/icons/icon-menu.svg') no-repeat;
    left: 20px;
    top: 25px;
    background-size: contain;
  }

  h1 {
    letter-spacing: 2px;
    // flex: 5;
  }

  h1:hover {
    transform: rotate(8deg);
    transition: 0.3s ease-in-out;
  }
}
</style>

