<template>
  <main-page />
</template>

<script>
import MainPage from './views/MainPage.vue';

export default {
  name: 'App',

  components: {
    MainPage,
  },
};
</script>

<style lang="scss">
@import url('https://cdn.jsdelivr.net/gh/orioncactus/pretendard@v1.3.5/dist/web/static/pretendard.css');
@import url('https://fonts.googleapis.com/css2?family=Urbanist:wght@700&display=swap');
@import './assets/styles.scss';
</style>
