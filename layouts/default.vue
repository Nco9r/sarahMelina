<template>
  <div>

    <nuxt />
    <the-footer/>
  </div>
</template>

<script>
import { gsap } from 'gsap'
import { ScrollTrigger } from 'gsap/dist/ScrollTrigger'
import TheFooter from '../components/Default/TheFooter.vue'
gsap.registerPlugin(ScrollTrigger)


export default {
  components: {
    TheFooter
 
  },
}
</script>

<style>
html {
  font-family: lato, Times, serif, -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  overflow-x: hidden;
}


*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}
body {
    overflow-x: hidden;
}
:root {
  --rose: #FFD9DF;
  --rose-secondary: #FD9FAE;
  --redBody: #9c3135; 
  --green: #D3E9E7; 
  --green-rhum: #155323; 
  --body: #4e4e4e;
  --gray-secondary: #afafaf;
  --white: #fff;
  --gray: #EFEFEF;
  --bleu: #2CA2B3;
  --black: #202020;
  --yellow: #F8ED63;
}

.btn button {
  background-color: var(--rose);
  color: var(--black);
  padding: 12px 24px;
  border: none;
  appearance: none;
  border-radius: 20px;
  font-weight: 900;
  width: 180px;
  font-size: 16px;
  margin: 15px 0;
}

@media  screen and (min-width: 768px) {
  body {
    display: none;
  }
}







</style>
