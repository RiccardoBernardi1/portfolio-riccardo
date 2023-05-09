<script>
import HeaderNav from "./HeaderNav.vue";
export default {
  name: "AppHeader",
  components: {
    HeaderNav,
  },
};
</script>

<template>
  <header>
    <HeaderNav />
  </header>
</template>

<style lang="scss" scoped>
header {
  background-color: #18181b;
  position: fixed;
  width: 100%;
  z-index: 100;
}
</style>
