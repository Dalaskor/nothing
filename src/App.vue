<template>
<HeaderView/>
</template>

<script>
import HeaderView from './components/HeaderView.vue';

export default {
  name: 'App',
  components: {
    HeaderView,
  },
};
</script>

<style lang="scss">
*{padding: 0;margin: 0;border: 0;}
*,*:before,*:after{-moz-box-sizing: border-box;-webkit-box-sizing: border-box;
box-sizing: border-box;}
:focus,:active{outline: none;}
a:focus,a:active{outline: none;}
nav,footer,header,aside{display: block;}
html,body{height: 100%;width: 100%;font-size: 100%;line-height: 1;font-size: 14px;
-ms-text-size-adjust: 100%;-moz-text-size-adjust: 100%;-webkit-text-size-adjust: 100%;}
input,button,textarea{font-family: inherit;}
input::-ms-clear{display: none;}
button{cursor: pointer;}
button::-moz-focus-inner{padding: 0;border: 0;}
a, a:visited{text-decoration: none;}
a:hover{text-decoration: none;}
ul li{list-style: none;}
img{vertical-align: top;}

@font-face {
  font-family: 'Inconsolata';
  font-display: swap;
  src: url("./assets/fonts/Inconsolata-SemiCondensed/Inconsolata-SemiCondensed-Regular.woff")
    format("woff");
  font-weight: 400;
  font-style: normal;
}
@font-face {
  font-family: 'Dot Matrix';
  font-display: swap;
  src: url("./assets/fonts/Dot-Matrix/DOTMATRI.TTF") format("truetype");
  font-weight: 400;
  font-style: normal;
}

[class*="__container"] {
  max-width: 1347px; // Ширина контейнера в макете + 15px * 2 из padding
  margin: 0px auto;
  padding: 0px 15px; // Отступы безопасности для адаптива
}

#app {
  font-family: 'Inconsolata';
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  line-height: 100%;
  color: #000000;
}
</style>
