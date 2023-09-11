<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppTopFooter from './components/AppTopFooter.vue';
import AppFooter from './components/AppFooter.vue';
import AppCard from './components/AppCard.vue';

export default {
  data() {
    return {};
  },

  components: { AppHeader, AppMain, AppCard, AppTopFooter, AppFooter },
};
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppCard />
  <AppTopFooter />
  <AppFooter />
</template>

<style lang="scss">
@use './styles/reset.scss' as *;
@use './styles/general.scss' as *;
</style>
