<template>
  <div>
    <nav class="ANav">
      <ul>
        <li><a href="#Home" id="MHome" class="active">Home</a></li>
        <li><a href="#Projects" id="MProjects">Projects</a></li>
        <li><a href="#About" id="MAbout">About</a></li>
      </ul>
    </nav>

    <div class="Home" id="Home">
      <svg version="1.1" id="Calque_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
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
</svg>
      <h1><span>B</span>ENJAMIN <span>S</span>CHINKEL</h1>
    </div>
    <div class="Projects" id="Projects">
      <div class="img-slider">
        <div class="navigation">
          <div class="btn open"></div>
          <div class="btn"></div>
          <div class="btn"></div>
          <div class="btn"></div>
          <div class="btn"></div>
        </div>
        <a href="http://faqmmimontbeliard.hirocitron.fr/" target="_blank">
          <div class="slide visible">
            <img src="../assets/img/affiche_1.jpg"
                 alt="FAQ MMi Montbéliard">
            <div class="info">
              <h2>FAQ MMi Montbéliard</h2>
              <p>Integration of the Montbéliard MMi FAQ with the Wordpress CMS.</p>
            </div>
          </div>
        </a>
        <a href="#" target="_blank">
          <div class="slide">
            <img src="../assets/img/affiche_2.jpg" alt="Setup de rêve">
            <div class="info">
              <h2>YOUR DREAM SETUP</h2>
              <p>Realization of most of the 3D parts of the setup with Blender.</p>
            </div>
          </div>
        </a>
        <a href="#" target="_blank">
          <div class="slide">
            <img src="../assets/img/affiche_3.jpg" alt="Groupe de TP">
            <div class="info">
              <h2>DRAW YOUR TP GROUP</h2>
              <p>Vector creation of my TP group of 15 people.</p>
            </div>
          </div>
        </a>
        <a href="https://www.youtube.com/watch?v=xSSluyqAHp0" target="_blank">
          <div class="slide">
            <img src="../assets/img/affiche_4.jpg" alt="Annie Lasne">
            <div class="info">
              <h2>Interview</h2>
              <p>Realization of an interview for a live of the IUT, writer of questions, cameraman & editor.</p>
            </div>
          </div>
        </a>
        <a href="https://www.youtube.com/watch?v=L1b1C4750HQ" target="_blank">
          <div class="slide">
            <img src="../assets/img/affiche_5.jpg" alt="Lunatique">
            <div class="info">
              <h2>Lunatique</h2>
              <p>Creation of a short film, screenwriter, director, cameraman & editor.</p>
            </div>
          </div>
        </a>

      </div>
    </div>
    <div class="About" id="About">
      <p class="meet">Hello, I am Benjamin. A young French student in Multimedia
        and Internet Professions in Montbéliard, I am passionate
        about the WEB integration and audiovisual.</p>
      <div class="contact">
        <p class="accroche">Do not hesitate to contact me :</p>
        <form class="contact-form" @submit.prevent="sendEmail">
          <div class="Oneline">
            <div class="Name">
              <label class="formL">Name</label>
              <input type="text" name="user_name" placeholder="Enter your name..." required="Please, enter your name">
            </div>
            <div class="Email">
              <label class="formL">Email</label>
              <input type="email" name="user_email" placeholder="Enter your Email..."
                     required="Please, enter your email">
            </div>
          </div>
          <div class="Message">
            <label class="formL">Message</label>
            <textarea name="message" placeholder="Write your message..."
                      required="Please, write your message"></textarea>
          </div>
          <div class="BSend">
            <input type="submit" value="Send" class="Send">
          </div>
          <div class="reponse">
            <p class="reussite cacher">Your mail was send</p>
            <p class="erreur cacher">Error try again</p>
          </div>
        </form>
      </div>
      <footer>
        <p>© benjamin schinkel | <a
            href="https://drive.google.com/file/d/1zbscqlrcUYBynBv4EygYcOGxurcKdgJJ/view?usp=sharing"
            target="_blank">CV</a></p>
      </footer>
    </div>
  </div>
</template>

<script>
import emailjs from 'emailjs-com';

export default {
  name: 'Accueil',
  props: {},
  mounted: function () {
    this.load_scriptA()
    this.sendEmail()
  },
  methods: {

    load_scriptA() {
      let liens = document.querySelectorAll("nav ul li a");
      window.addEventListener('scroll', function () {
        if (window.pageYOffset <= (window.innerHeight - 1)) {
          liens[0].classList.add("active");
          liens[1].classList.remove("active");
          liens[2].classList.remove("active");
        } else if (window.innerHeight >= window.pageYOffset || window.pageYOffset <= (2 * window.innerHeight - 1)) {
          liens[1].classList.add("active");
          liens[0].classList.remove("active");
          liens[2].classList.remove("active");
        } else if ((2 * window.innerHeight) >= window.pageYOffset) {
          liens[2].classList.add("active");
          liens[0].classList.remove("active");
          liens[1].classList.remove("active");
        }
      });

      let slides = document.querySelectorAll('.slide');
      let btns = document.querySelectorAll('.btn');
      console.log(slides)
      console.log(btns)

      btns[0].addEventListener("click", function () {
        btns[0].classList.add("open");
        slides[0].classList.add("visible");
        btns[1].classList.remove("open");
        slides[1].classList.remove("visible");
        btns[2].classList.remove("open");
        slides[2].classList.remove("visible");
        btns[3].classList.remove("open");
        slides[3].classList.remove("visible");
        btns[4].classList.remove("open");
        slides[4].classList.remove("visible");
      });
      btns[1].addEventListener("click", function () {
        btns[1].classList.add("open");
        slides[1].classList.add("visible");
        btns[0].classList.remove("open");
        slides[0].classList.remove("visible");
        btns[2].classList.remove("open");
        slides[2].classList.remove("visible");
        btns[3].classList.remove("open");
        slides[3].classList.remove("visible");
        btns[4].classList.remove("open");
        slides[4].classList.remove("visible");
      });
      btns[2].addEventListener("click", function () {
        btns[2].classList.add("open");
        slides[2].classList.add("visible");
        btns[0].classList.remove("open");
        slides[0].classList.remove("visible");
        btns[1].classList.remove("open");
        slides[1].classList.remove("visible");
        btns[3].classList.remove("open");
        slides[3].classList.remove("visible");
        btns[4].classList.remove("open");
        slides[4].classList.remove("visible");
      });
      btns[3].addEventListener("click", function () {
        btns[3].classList.add("open");
        slides[3].classList.add("visible");
        btns[0].classList.remove("open");
        slides[0].classList.remove("visible");
        btns[1].classList.remove("open");
        slides[1].classList.remove("visible");
        btns[2].classList.remove("open");
        slides[2].classList.remove("visible");
        btns[4].classList.remove("open");
        slides[4].classList.remove("visible");
      });
      btns[4].addEventListener("click", function () {
        btns[4].classList.add("open");
        slides[4].classList.add("visible");
        btns[0].classList.remove("open");
        slides[0].classList.remove("visible");
        btns[1].classList.remove("open");
        slides[1].classList.remove("visible");
        btns[2].classList.remove("open");
        slides[2].classList.remove("visible");
        btns[3].classList.remove("open");
        slides[3].classList.remove("visible");
      });
    },

    sendEmail: (e) => {
      let reponses = document.querySelectorAll("div form div p");

      emailjs.sendForm('service_zllowae', 'template_dn8uswn', e.target, 'user_5LwLuFfYFuIbcTmo6uQhN')
          .then((result) => {
            console.log('SUCCESS!', result.status, result.text);
            reponses[0].classList.remove("cacher");
          }, (error) => {
            console.log('FAILED...', error);
            reponses[1].classList.remove("cacher");
          });
      e.target.reset();
    },
  }
}
</script>

<style scoped>

/* Background */

.Home, .About {
  height: 100vh;
  width: 100vw;
  background-color: #212121;
  position: relative;
}

.Projects {
  height: 100vh;
  width: 100vw;
  background-color: #FFF2E6;
  position: relative;
}

/* Menu */

nav li {
  list-style: none;
  margin: 1.3em 0.78em 1.3em 0;
}

.ANav {
  position: fixed;
  display: grid;
  right: 2.6em;
  top: 2.6em;
  z-index: 2;
}

.ANav a {
  font-size: 1.823em;
  text-decoration: none;
  color: #4D4D4D;
}

.ANav a.active {
  font-family: "caviar_dreamsbold", sans-serif;
  color: #FFCC00;
}

@media (max-width: 670px) {
  .ANav{display: none;}
}

/* Home */

.Home {
  text-align: center;
}

.Home svg {
  height: 50vh;
  margin: 25vh 0 0 0;
}

.st0 {
  fill: none;
  stroke: #FFF2E6;
  stroke-width: 10px;
  stroke-miterlimit: 10;
  stroke-dasharray: 2000;
  stroke-dashoffset: 2000;
  animation: dashben 3s linear forwards;
}

@keyframes dashben {
  to {
    stroke-dashoffset: 0;
  }
}

.st2 {
  fill: none;
  stroke: #FFF2E6;
  stroke-width: 10px;
  stroke-miterlimit: 10;
  opacity: 0;
  animation: dashpoly 3s linear forwards;
}

@keyframes dashpoly {
  to {
    opacity: 1;
  }
}

h1 {
  color: #FFF2E6;
  font-size: 5rem;
  opacity: 0;
  margin: 4rem;
  animation: dashtext 2s linear forwards;
}

@keyframes dashtext {
  to {
    opacity: 1;
    margin: 1rem;
  }
}

h1 span {
  color: #FFCC00;
}

@media (max-width: 500px) {
  .Home svg {
    height: 25vh;
    margin: 30vh 0 0 0;
    top: 50vh;
  }

  h1{
    font-size: 3em;
  }
}

/* PROJETS */

.Projects {
  display: flex;
  justify-content: center;
  align-items: center;
}

h2 {
  font-family: caviar_dreamsbold, sans-serif;
}

.img-slider {
  position: relative;
  width: 800px;
  height: 500px;
  margin: 10px;
  background: #FFF2E6;
}

.img-slider .slide {
  z-index: 1;
  position: absolute;
  width: 100%;
  clip-path: circle(0% at 0 50%);
}

.img-slider .slide.visible {
  clip-path: circle(150% at 0 50%);
  transition: 2s;
  transition-property: clip-path;
}

.img-slider .slide img {
  z-index: 1;
  width: 100%;
  border-radius: 5px;
}

.img-slider .slide .info {
  position: absolute;
  top: 0;
  padding: 15px 30px;
}

.img-slider .slide .info h2 {
  color: #FFF2E6;
  font-size: 45px;
  text-transform: uppercase;
  font-weight: 800;
  letter-spacing: 2px;
}

.img-slider .slide .info p {
  color: #FFF2E6;
  background: rgba(0, 0, 0, 0.1);
  font-size: 16px;
  width: 60%;
  padding: 10px;
  border-radius: 4px;
}

.img-slider .navigation {
  z-index: 2;
  position: absolute;
  display: flex;
  bottom: 30px;
  left: 50%;
  transform: translateX(-50%);
}

.img-slider .navigation .btn {
  background: rgba(77, 77, 77, 0.5);
  width: 12px;
  height: 12px;
  margin: 10px;
  border-radius: 50%;
  cursor: pointer;
}

.img-slider .navigation .btn.open {
  background: #FFCC00;
  box-shadow: 0 0 2px rgba(0, 0, 0, 0.5);
}

@media (max-width: 820px) {
  .img-slider {
    width: 600px;
    height: 375px;
  }

  .img-slider .slide .info {
    padding: 10px 25px;
  }

  .img-slider .slide .info h2 {
    font-size: 35px;
  }

  .img-slider .slide .info p {
    width: 70%;
    font-size: 15px;
  }

  .img-slider .navigation {
    bottom: 25px;
  }

  .img-slider .navigation .btn {
    width: 10px;
    height: 10px;
    margin: 8px;
  }
}

@media (max-width: 620px) {
  .img-slider {
    width: 400px;
    height: 250px;
  }

  .img-slider .slide .info {
    padding: 10px 20px;
  }

  .img-slider .slide .info h2 {
    font-size: 30px;
  }

  .img-slider .slide .info p {
    width: 80%;
    font-size: 13px;
  }

  .img-slider .navigation {
    bottom: 15px;
  }

  .img-slider .navigation .btn {
    width: 8px;
    height: 8px;
    margin: 6px;
  }
}

@media (max-width: 420px) {
  .img-slider {
    width: 320px;
    height: 200px;
  }

  .img-slider .slide .info {
    padding: 5px 10px;
  }

  .img-slider .slide .info h2 {
    font-size: 25px;
  }

  .img-slider .slide .info p {
    width: 90%;
    font-size: 11px;
  }

  .img-slider .navigation {
    bottom: 10px;
  }
}

/* About */

.About {
  position: relative;
}

.About p.meet {
  font-size: 3rem;
  color: #FFF2E6;
  margin: 0 15vw 0 30vw;
  text-align: right;
  border-right: 5px solid #4D4D4D;
  padding-right: 1rem;
  position: absolute;
  top: 5vh;
}

.About p.accroche {
  font-size: 3rem;
  color: #FFF2E6;
  position: absolute;
  top: 25vh;
  left: 10vw;
}

.About label.formL {
  display: none;
}

.About input, textarea {
  font-family: "caviar_dreamsregular", sans-serif;
  background-color: #212121;
  border: none;
  border-bottom: 1px solid #4D4D4D;
  color: #FFF2E6;
  margin: 1em;
  font-size: 1.5em;
}

.About input {
  height: 5vh;
  width: 34vw;
}

.About .BSend {
  text-align: right;
}

.About input.Send {
  color: #FFF2E6;
  border: 1px solid #FFF2E6;
  background-color: #4D4D4D;
  width: 5vw;
  padding: 1vh;
  border-radius: 100px;
}

.About form {
  position: absolute;
  top: 35vh;
  left: 10vw;
}

.About .Oneline {
  display: inline-flex;
}

.About textarea {
  height: 30vh;
  width: 70vw;
  resize: none;
}

.erreur, .reussite {
  font-size: 1.5em;
  font-family: caviar_dreamsbold, sans-serif;
  color: #FFCC00;
  background-color: #212121;
  display: inline;
  padding: 0 10px;
}

.cacher {
  display: none;
}

@media (max-width: 1120px) {
  .About p.meet {
    font-size: 20px;
  }

  .About p.accroche{
    font-size: 20px;
  }
}

@media (max-width: 940px) {
  .About input, textarea {
    font-size: 12px;
  }

  .About input.Send {
    width: auto;
    padding: 5px;
  }

  .erreur, .reussite {
    font-size: 12px;
  }
}

@media (max-width: 780px) {
  .About p.meet {
    margin: 0 15vw 0 15vw;
  }
}

@media (max-width: 670px) {
  .About p.meet {
    margin: 0 5vw 0 20vw;
  }
}

@media (max-width: 450px) {
  .About p.meet {
    font-size: 15px;
    margin: 0 5vw 0 30vw;
  }

  .About p.accroche{
    font-size: 15px;
    top: 28vh;
  }
}

/* FOOTER */

footer {
  position: absolute;
  bottom: 0;
  left: 40vw;
  padding: 3vh;
}

footer p {
  color: #FFF2E6;
  margin: 0;
  font-size: 1.5vw;
}

footer p a {
  color: #FFCC00;
  text-decoration: none;
}

footer p a:hover {
  font-family: caviar_dreamsbold, sans-serif;
}

@media (max-width: 800px) {
  footer{
    margin: 0 30vw;
    left: 0;
  }

  footer p{
    font-size: 15px;
  }
}

</style>
