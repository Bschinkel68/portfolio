<template>
  <div id="app">
    <Accueil/>
    <nav class="HRSNav" id="RS">
      <span><a class="interact"><svg version="1.1" id="Calque_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
           x="0px"
           y="0px"
           viewBox="0 0 1500 1500" style="enable-background:new 0 0 1500 1500;" xml:space="preserve">

        <g id="Logo">
        <!-- B -->
        <path class="st0" d="M596.94,460.47c0-116.55-97.88-211.04-214.43-211.04l-0.01,422.03c1.13,0.02,2.27,0.04,3.4,0.04
		C502.45,671.51,596.94,577.02,596.94,460.47z M382.5,671.46v574.16c157.77,0,285.67-128.53,285.67-287.08S540.27,671.46,382.5,671.46z"/>
          <!-- E -->
          <line class="st0" x1="382.51" y1="249.4" x2="742.29" y2="249.4"/>
          <polyline class="st0" points="382.5,671.46 742.29,671.46 1102.06,671.46"/>
          <line class="st0" x1="382.51" y1="1245.63" x2="742.29" y2="1245.63"/>
          <!-- N -->
          <line class="st0" x1="382.51" y1="249.4" x2="742.29" y2="1245.63"/>
          <line class="st0" x1="742.29" y1="249.4" x2="742.29" y2="1247.8"/>
          <!-- J -->
          <path class="st0" d="M1102.06,249.4v422.11v279.75c0,0-0.63,294.37-180.2,294.37S742.29,951.26,742.29,951.26"/>
          <!-- M -->
          <line class="st0" x1="742.29" y1="249.4" x2="1102.06" y2="1245.63"/>
          <!-- I -->
          <line class="st0" x1="1102.06" y1="1245.63" x2="1102.06" y2="671.51"/>
          <!-- Hexagone -->
          <polygon class="st2"
                   points="94.73,377.25 94.73,1124.98 742.29,1498.85 1389.85,1124.98 1389.85,377.25 742.29,3.38 94.73,377.25"/>
</g>
</svg></a></span>
      <a href="https://www.linkedin.com/in/benjamin-schinkel-873546195/" class="hide moi" target="_blank"><i
          class="fa fa-linkedin" aria-hidden="true"></i></a>
      <a href="https://www.instagram.com/benjaminschinkel/" class="hide moi" target="_blank"><i class="fa fa-instagram"
                                                                                             aria-hidden="true"></i></a>
      <a href="https://twitter.com/BenjaminSch6" class="hide moi" target="_blank"><i class="fa fa-twitter"
                                                                                  aria-hidden="true"></i></a>
      <a href="https://www.facebook.com/benjamin.schinkel.68/" class="hide moi" target="_blank"><i class="fa fa-facebook"
                                                                                                aria-hidden="true"></i></a>
    </nav>
    <div id="progressbar"></div>
    <div id="scrollPath"></div>
  </div>
</template>

<script>
import Accueil from './components/Accueil.vue'

export default {
  name: 'App',
  components: {
    Accueil
  },
  mounted: function () {
    this.load_script()
  },
  methods: {
    load_script() {
      let progress = document.getElementById('progressbar');
      let totalHeight = document.body.scrollHeight - window.innerHeight;
      window.onscroll = function () {
        let progressHeight = (window.pageYOffset / totalHeight) * 100;
        progress.style.height = progressHeight + "%";
      }
      let svgb = document.querySelectorAll('.interact');
      let amoi = document.querySelectorAll('.moi');
      console.log(amoi)
      svgb[0].addEventListener('click',() => {
        amoi[0].classList.toggle('hide');
        amoi[1].classList.toggle('hide');
        amoi[2].classList.toggle('hide');
        amoi[3].classList.toggle('hide');
      });
    }
  }
}
</script>

<style>
/* Default */

html, body {
  margin: 0;
}

html {
  font-size: 62.5%;
  font-family: "caviar_dreamsregular", sans-serif;
  position: relative;
}

/* Fonts */

@font-face {
  font-family: 'caviar_dreamsbold';
  src: url('assets/fonts/caviardreams_bold-webfont.woff2') format('woff2'),
  url('assets/fonts/caviardreams_bold-webfont.woff') format('woff');
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: 'caviar_dreamsregular';
  src: url('assets/fonts/caviardreams-webfont.woff2') format('woff2'),
  url('assets/fonts/caviardreams-webfont.woff') format('woff');
  font-weight: normal;
  font-style: normal;
}

/* Home & RS Nav */

.HRSNav {
  position: fixed;
  display: grid;
  left: 2.6em;
  top: 2.6em;
  justify-items: center;
  z-index: 2;
  margin-top: 1.3em;
}

.HRSNav a.moi{
  font-size: 1.56vw;
  text-decoration: none;
  color: #4D4D4D;
  height: 1.56vw;
  width: 1.56vw;
  margin: 0.65vw 0;
  padding: 0.52vw;
  border-radius: 50%;
  border: 1px solid #4D4D4D;
  transition: 0.3s;
  text-align: center;
}

.HRSNav a.moi:hover {
  font-family: "caviar_dreamsbold", sans-serif;
  color: #FFCC00;
  font-size: 3.12vw;
  height: 3.12vw;
  width: 3.12vw;
  border-color: #FFCC00;
  text-align: center;
}

.HRSNav svg {
  height: 60px;
  width: 60px;
  margin-bottom: 10px;
}

.st0 {
  fill: none;
  stroke: #FFCC00;
  stroke-width: 30px;
  height: 2vw;
  width: 2vw;
}

.st2 {
  fill: none;
  stroke: #FFCC00;
  stroke-width: 30px;
  stroke-miterlimit: 10;
}

a.hide{
  display: none;
}

@media (max-width: 800px) {
  .HRSNav a.moi{
    font-size: 20px;
    height: 20px;
    width: 20px;
    margin: 5px 0;
    padding: 2.5px;
  }

  .HRSNav a.moi:hover{
    font-size: 30px;
    height: 30px;
    width: 30px;
    margin: 10px 0;
    padding: 5px;
  }
}

/* Scrollbar */

::-webkit-scrollbar {
  width: 0;
}

#scrollPath {
  position: fixed;
  top: 0;
  right: 0;
  width: 10px;
  height: 100vh;
  background: rgba(0, 0, 0, 0.1);
}

#progressbar {
  position: fixed;
  top: 0;
  right: 0;
  width: 10px;
  background: linear-gradient(to top, #FFCC00, #FFCC00);
  animation: animate 5s linear infinite;
}

@keyframes {
  0%, 100% {
    filter: hue-rotate(0deg);
  }
  50% {
    filter: hue-rotate(360deg);
  }
}

/* GLOW EFFECT

#progressbar:before{
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(to top, #FFCC00, #FFCC00);
  filter: blur(10px);
}

#progressbar:after{
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(to top, #FFCC00, #FFCC00);
  filter: blur(30px);
}

*/
</style>
