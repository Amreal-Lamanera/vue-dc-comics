<template>
  <footer>
    <FooterHeader/>
    <FooterMain/>
    <FooterFooter/>
  </footer>
</template>

<script>
import FooterHeader from "./FooterHeader.vue";
import FooterMain from "./FooterMain.vue";
import FooterFooter from "./FooterFooter.vue";
export default {
    components: { FooterHeader, FooterMain, FooterFooter }
}
</script>

<style lang="scss" scoped>

</style>