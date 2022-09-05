<template>
  <div id="app">
    <MainHeader/>
    <MainComponent/>
    <MainFooter/>
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue';
import MainComponent from './components/MainComponent.vue';
import MainFooter from './components/MainFooter.vue';

export default {
  name: 'App',
  components: {
    MainHeader,
    MainComponent,
    MainFooter
}
}
</script>

<style lang="scss">

@import '@/style/index.scss';

</style>
