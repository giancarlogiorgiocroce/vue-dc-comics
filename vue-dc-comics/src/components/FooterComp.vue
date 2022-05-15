<template>
  <footer>
    <FooterUp />
    <FooterDown />
  </footer>
</template>

<script>
import FooterDown from "./FooterDown.vue";
import FooterUp from "./FooterUp.vue";
export default {
    components: { FooterDown, FooterUp }
}
</script>

<style lang="scss" scoped>

</style>