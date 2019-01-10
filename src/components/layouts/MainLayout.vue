<template>
  <a-layout>
    <main-sider/>
    <a-layout style="padding-left:256px;min-height:100vh;">
      <main-header/>
      <a-layout-content>
        <router-view />
      </a-layout-content>
      <main-footer/>
    </a-layout>
  </a-layout>
  <!-- <transition name="page-transition">
    <keep-alive v-if="keepAlive">
      <router-view />
    </keep-alive>
    <router-view v-else />
  </transition> -->
</template>
<script>
import mainSider from './main/Sider'
import mainHeader from './main/Header'
import mainFooter from './Footer'
export default {
  name: 'MainLayout',
  components: { mainSider, mainHeader, mainFooter },
  data() {
    return {
    }
  },
  computed: {
    // keepAlive() {
    //   return this.$route.meta.keepAlive
    // }
  },
  methods: {
  }
}
</script>
<style scoped>
/* .ant-layout {
} */
.ant-layout .ant-layout-content {
  padding-top:64px;
  height:100%;
}
</style>