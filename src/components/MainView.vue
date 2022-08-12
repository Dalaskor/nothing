<template>
<main class="main">
    <HomeView/>
    <FeaturesView/>
</main>
</template>

<script>
import HomeView from './HomeView.vue';
import FeaturesView from './FeaturesView.vue';

export default {
  name: 'MainView',
  components: {
    HomeView,
    FeaturesView,
  },
};
</script>

<style scoped lang="scss">
</style>
