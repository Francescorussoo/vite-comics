<template>
  <div id="app">
    <!-- Header component -->
    <AppHeader />

    <!-- Main content component -->
    <AppMain />

    <!-- Comic List component -->
    <ComicList />

    <!-- App Footer component -->
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import ComicList from './components/ComicList.vue';

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    ComicList,
    AppFooter
  },
  data() {
    return {
    };
  },
  methods: {
    IncrementCount() {
      this.count++;
    }
  }
}
</script>

<style lang="scss" scoped>
body {
  font-family: 'Arial', sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f0f0f0;
}
</style>
