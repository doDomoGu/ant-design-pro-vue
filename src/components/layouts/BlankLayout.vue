<template>
  <a-layout>
    <a-layout-content>
      <router-view />
    </a-layout-content>
    <my-footer />
  </a-layout>
</template>

<script>
import MyFooter from './Footer'
export default {
  name: 'BlankLayout',
  components: { MyFooter },
}
</script>
<style scoped>
.ant-layout {
  min-height: 100vh;
}
.ant-layout .ant-layout-content {
  height:100%;
}

</style>