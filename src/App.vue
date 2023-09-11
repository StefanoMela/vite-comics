<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppTopFooter from './components/AppTopFooter.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  data() {
    return {};
  },

  components: { AppHeader, AppMain, AppTopFooter, AppFooter },
};
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppTopFooter />
  <AppFooter />
</template>

<style lang="scss">
@use './styles/reset.scss' as *;
@use './styles/general.scss' as *;
</style>
