<template>
  <div id="app">
    <VHeader></VHeader>
    <AsideMenu></AsideMenu>
  </div>
</template>

<script>
import VHeader from './components/Header'
import AsideMenu from './components/AsideMenu'
export default {
  name: 'app',
  components: {
    VHeader,
    AsideMenu
  }
}
</script>

<style>
@import "./common/style/base.scss";
#app {
  display: flex;
  flex-direction: column;
  width: 100%;
  height: 100%;
}
</style>
