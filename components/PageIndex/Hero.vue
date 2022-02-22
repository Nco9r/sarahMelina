<template>
  <main class="attente">
    <div class="hero_content">
      <div class="content_hero">
        <h1>CRÉATRICE DE CONTENU <span class="after">CULINAIRE</span></h1>
        <p>
          J’accompagne les professionnels de la restauration dans la gestion de
          leur image sur internet, à Bordeaux et dans la France entière.
        </p>
        <div class="btn">
            <button>Devis gratuit</button>
        </div>
        <a href="https://www.facebook.com/bysarahmelina/" target="_blank">
          <img src="~assets/img/svg/fb.svg" alt="" />
        </a>
        <a
          href="https://www.instagram.com/by_sarahmelina/?hl=fr"
          target="_blank"
        >
          <img src="~assets/img/svg/insta.svg" alt="" />
        </a>
        <a
          href="https://fr.linkedin.com/in/sarah-da-silva-94823017b"
          target="_blank"
        >
          <img src="~assets/img/svg/lin.svg" alt="" />
        </a>
      </div>
    </div>
    <div class="scroll">
      <p>Scroll</p>
      <img src="~assets/img/svg/scroll.svg" alt="">
    </div>
  </main>
</template>

<script>
export default {}
</script>

<style scoped>
main {
  width: 100%;
  height: 100vh;
  background-image: url('~assets/img/jpg/home.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  flex-flow: column;
  align-items: flex-end;
  position: relative;
  background-position: 60%;
}


.content_hero {
  margin-top: 100px;
  padding: 0 20Px 0 50px;
  text-align: center;
}

.content_hero h1 {
  font-size: 26px;
  margin-bottom: 10px;
  font-weight: 900!important;
}

.content_hero p {
  padding: 5px 45px;
  font-size: 16px;
  margin: auto;
  width: 360px;
  line-height: 26px;
  color: rgb(78, 78, 78);
}

.after::after {
  content: '';
  position: relative;
  background-color: var(--rose);
  width: 100%;
  height: 13Px;
  left: 0;
}

.content_hero img {
  margin-top: 20px;
}

.scroll {
  position: absolute; 
  bottom: 20px;
  margin: auto;
  left: 50%;
  transform: translateX(-50%);
}

.scroll p {
  margin-bottom: 45px;
  margin-left: -12px;
  font-size: 12px;
  text-transform: uppercase;
  font-weight: 900;
  transform: rotate(-90deg);
}

.scroll img {
  animation: scroll 1.5s infinite;
}

@keyframes scroll {
  0% {
    transform: translateY(0);
  }
   50% {
    transform: translateY(-20px);
  } 100% {
    transform: translateY(0);
  }
}

@media screen and (min-width: 1024px) {
  .attente {
    text-align: center;
  }

  .hero_content {
    margin-right: 50px;
  }

  .content_hero h1 {
    font-size: 36px;
    margin-bottom: 20px;
  }

  .content_hero p {
    padding: 15px 5px;
    font-size: 18px;
    width: 500px;
    line-height: 32px;
    color: rgb(78, 78, 78);
  }
}

@media screen and (min-width: 1200px) {
  .attente {
    text-align: center;
  }

  .hero_content {
    margin-right: 50px;
  }

  .content_hero h1 {
    font-size: 36px;
    margin-bottom: 20px;
  }

  .content_hero p {
    padding: 15px 5px;
    font-size: 18px;
    width: 600px;
    line-height: 32px;
    color: rgb(78, 78, 78);
  }
}

@media screen and (min-width: 1600px) {
  .attente {
    text-align: center;
  }

  .hero_content {
    margin-right: 200px;
  }

  .content_hero h1 {
    font-size: 46px;
    margin-bottom: 20px;
  }

  .content_hero p {
    padding: 15px 5px;
    font-size: 22px;
    width: 750px;
    line-height: 36px;
    color: rgb(78, 78, 78);
  }
}
</style>
