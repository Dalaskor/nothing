<template>
<main class="main" id="main">
    <HomeView/>
    <FeaturesView/>
    <SoundView/>
</main>
</template>

<script>
import HomeView from './HomeView.vue';
import FeaturesView from './FeaturesView.vue';
import SoundView from './SoundView.vue';

export default {
  name: 'MainView',
  components: {
    HomeView,
    FeaturesView,
    SoundView,
  },
};
</script>

<style scoped lang="scss">
</style>
