<template lang="html">
  <transition name="slide-left">
    <div class="aside-menu">
      <div class="menu">
        <div class="user">
          <div class="user-avatar">
            <img src="http://omratag7g.bkt.clouddn.com/icon-unlogin.svg" alt="">
          </div>
          <div class="user-name">
            点击头像登录
          </div>
        </div>
        <div class="infos">
          <div class="block">
            <i class="icon-msg"></i>
            我的消息
          </div>
          <div class="block">
            <i class="icon-new"></i>
            发布话题
          </div>
          <div class="block">
            <i class="icon-info"></i>
            个人中心
          </div>
          <div class="block">
            <i class="icon-about"></i>
            关于
          </div>
          <div class="cnode"></div>
        </div>
      </div>
      <div class="mask"></div>
    </div>
  </transition>
</template>

<script>
  export default {
    name: 'asideMenu',
    methods: {

    },
    computed: {
    }
  }
</script>

<style lang="scss" scoped>
  .aside-menu {
    display: flex;
    position: absolute;
    left: 0;
    right: 0;
    bottom: 0;
    top: 0;
    z-index: 1;
    .menu {
      display: flex;
      width: 220px;
      background-color: #fff;
      box-shadow: 0 0 12px gray;
      flex-direction: column;
      .user {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 100%;
        height: 200px;
        background-color: #2196F3;
        color: white;
        .user-avatar {
          img {
            width: 100px;
            height: 100px;
            border-radius: 50px;
            cursor: pointer;
          }
        }
        .user-name {
          font-size: 1.2rem;
        }
      }
      .infos {
        display: flex;
        flex-direction: column;
        align-items: center;
        flex: 1;
        .block {
          width: 100%;
          height: 50px;
          padding-left: 50px;
          cursor: pointer;
          display: flex;
          align-items: center;
        }
        .block + .block {
          border-top: 1px solid rgba(0, 0, 0, .05);
        }
        i {
          display: inline-block;
          width: 22px;
          height: 22px;
          background-repeat: no-repeat;
          margin-right: 8px;
        }
        .icon-msg {
          background: url('../common/icons/icon-msg-blue.svg');
          background-size: contain;
        }
        .icon-new {
          background: url('../common/icons/icon-new.svg');
          background-size: contain;
        }
        .icon-about {
          background: url('../common/icons/icon-about.svg');
          background-size: contain;
        }
        .icon-info {
          background: url('../common/icons/icon-info.svg');
          background-size: contain;
        }
        .cnode {
          margin-top: 150px;
          width: 50%;
          height: 100px;
          background: url('../common/icons/icon-cnode.svg') no-repeat;
          // background-color: pink;
          background-size: contain;
          opacity: 0.3;
          flex: 1;
        }
      }
    }
    .mask {
      flex: 1;
      // background-color: red;
    }
  }
</style>