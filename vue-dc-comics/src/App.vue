<template>
  <div id="app">
    <HeaderComp />
    <JumboComp />
    <MainComp />
    <BlueStripe />
    <FooterComp />
  </div>
</template>

<script>
import HeaderComp from "./components/HeaderComp.vue";
import JumboComp from "./components/JumboComp.vue";
import MainComp from "./components/MainComp.vue";
import BlueStripe from "./components/BlueStripe.vue";
import FooterComp from "./components/FooterComp.vue";

export default {
  name: 'App',
  components: {
    HeaderComp,
    JumboComp,
    MainComp,
    BlueStripe,
    FooterComp,
}
}
</script>

<style lang="scss">
@import 'assets/style/vars.scss';
@import 'assets/style/global.scss';
@import 'assets/style/utils.scss';

</style>
