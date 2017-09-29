<template>
  <div id="pageQuiButton">
    <p style="color: #ccc; font-size: 12">开发组件库</p>
    <qui-btn msg='确定' v-on:btnClickEvent='doSth'></qui-btn>
    <qui-btn msg='取消' v-on:btnClickEvent='doSth1'></qui-btn>
    <qui-btn msg='下载'>
      <img src="../assets/logo.png" alt="" slot="icon">
    </qui-btn>
  </div>
</template>

<script>
import quiBtn from '@/components/quiButton.vue'
export default {
  name: 'pageQuiButton',
  components: {
    'qui-btn': quiBtn
  },
  methods: {
    doSth () {
      alert('你点击了组件的click: btnClickEvent111')
    },
    doSth1 () {
      alert('你点击了组件的click: btnClickEvent222')
    }
  }
}
</script>
<style>
  #pageQuiButton {
    width: 100px;
    height: 300px;
    background-color: red;
    margin-right: 100px;
    border: 1px solid blue;
  }
</style>

