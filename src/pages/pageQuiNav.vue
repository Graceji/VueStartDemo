<template>
  <qui-nav v-on:navClickEvent="navClickEvent" :items="items"></qui-nav>
</template>

<script>
import quiNav from '@/components/quiNav.vue'
export default {
  data () {
    return {
      items: [
        {
          text: '首页',
          active: true
        },
        {
          text: '列表',
          active: false
        },
        {
          text: '关于',
          active: false
        },
        {
          text: '招聘',
          active: false
        }
      ]
    }
  },
  methods: {
    navClickEvent (items, index) {
      console.log(index)
      items.forEach(item => {
        item.active = false
      })
      items[index].active = true
    }
  },
  components: {
    'qui-nav': quiNav
  }
}
</script>


