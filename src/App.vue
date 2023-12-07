<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import SectionShop from './components/SectionShop.vue';

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    AppFooter,
    SectionShop,
  },
};
</script>

<template>
  <AppHeader />
  <AppMain />
  <SectionShop />
  <AppFooter />
</template>

<style lang="scss">
@use './styles/general' as *;
@use './styles/common' as *;
</style>
