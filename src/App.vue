<template>
  <div id="app">
    <v-svg type="Cancel" :is-disable="true" />
    <v-svg type="Cancel" />
    <img src="./assets/logo.png">
    <img class="cancelBtn" svg-inline src="./assets/img/normal.svg">
    <img class="cancelBtnDisable" svg-inline src="./assets/img/normal.svg">
    <normal />
    <svg width="93px" height="48px" viewBox="0 0 93 48" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
        <!-- Generator: Sketch 51.1 (57501) - http://www.bohemiancoding.com/sketch -->
        <title>btn/main/cancel/normal</title>
        <desc>Created with Sketch.</desc>
        <defs></defs>
        <g id="btn/main/cancel/normal" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
            <rect id="Rectangle-3" fill-rule="nonzero" x="0" y="0" width="93" height="48"></rect>
            <text id="CANCEL" font-family="Roboto" font-size="16" font-weight="bold" fill="#787878">
                <tspan x="16.1679688" y="27">CANCEL</tspan>
            </text>
        </g>
    </svg>
    <HelloWorld/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import VSvg from './components/VSvg'
import normal from './assets/img/normal.svg'

export default {
  name: 'App',
  components: {
    HelloWorld,
    VSvg,
    normal
  }
}
</script>

<style>

@font-face {
  font-family: 'Roboto';
  src: url('./assets/fonts/Roboto-Regular.ttf');
}

#app {
  font-family: 'Roboto';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.cancelBtn:hover g {
  fill: #F5F5F5;
}

.cancelBtnDisable text {
  fill: #C8C8C8;
}
</style>
