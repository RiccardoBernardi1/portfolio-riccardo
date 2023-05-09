<template>
  <div id="homepage">
    <AppHeader />
    <AppMain />
  </div>
</template>

<script>
import AppHeader from "../components/Header/AppHeader.vue";
import AppMain from "../components/Main/AppMain.vue";
export default {
  name: "Homepage",
  components: {
    AppHeader,
    AppMain,
  },
};
</script>

<style lang="scss" scoped>
#homepage {
  background: linear-gradient(-45deg, #a0470c, #49176d, #185db8, #23d5ab);
  background-size: 1000% 1000%;
  animation: gradient 15s ease infinite;
  height: 100%;
}

@keyframes gradient {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}
</style>
