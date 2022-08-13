<template>
<main class="main" id="main">
    <HomeView/>
    <FeaturesView/>
    <SoundView/>
    <TonesView/>
</main>
</template>

<script>
import HomeView from './HomeView.vue';
import FeaturesView from './FeaturesView.vue';
import SoundView from './SoundView.vue';
import TonesView from './TonesView.vue';

export default {
  name: 'MainView',
  components: {
    HomeView,
    FeaturesView,
    SoundView,
    TonesView,
  },
};
</script>

<style scoped lang="scss">
</style>
