<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
  },
};
</script>

<style lang="scss">
@font-face {
	font-family: 'Inconsolata';
	font-display: swap;
	src: url("./assets/fonts/Inconsolata-SemiCondensed/Inconsolata-SemiCondensed-Regular.woff") format("woff");
	font-weight: 400;
	font-style: normal;
}
@font-face {
	font-family: 'Dot Matrix';
	font-display: swap;
	src: url("./assets/fonts/Dot-Matrix/DOTMATRI.TTF") format("ttf");
	font-weight: 400;
	font-style: normal;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
