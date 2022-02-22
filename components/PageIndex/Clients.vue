<template>
  <section class="client">
    <div class="box_client">
      <img class="photof" src="~assets/img/svg/photof.svg" alt="" />
      <img class="tocf" src="~assets/img/svg/tocf.svg" alt="" />
      <div class="content">
        <img src="~assets/img/svg/arrow.svg" alt="" />
        <h3>Ils me font <span>confiance !</span></h3>
      </div>
    </div>
    <section class="partenaires">
      <div class="box">
        <img src="~assets/img/svg/pq.svg" alt="" />
        <img src="~assets/img/svg/avo.svg" alt="" />
        <img src="~assets/img/svg/qc.svg" alt="" /><img
          src="~assets/img/svg/pq.svg"
          alt=""
        />
        <img src="~assets/img/svg/avo.svg" alt="" />
        <img src="~assets/img/svg/qc.svg" alt="" /><img
          src="~assets/img/svg/pq.svg"
          alt=""
        />
        <img src="~assets/img/svg/avo.svg" alt="" />
        <img src="~assets/img/svg/qc.svg" alt="" /><img
          src="~assets/img/svg/pq.svg"
          alt=""
        />
        <img src="~assets/img/svg/avo.svg" alt="" />
        <img src="~assets/img/svg/qc.svg" alt="" /><img
          src="~assets/img/svg/pq.svg"
          alt=""
        />
        <img src="~assets/img/svg/avo.svg" alt="" />
        <img src="~assets/img/svg/qc.svg" alt="" /><img
          src="~assets/img/svg/pq.svg"
          alt=""
        />
        <img src="~assets/img/svg/avo.svg" alt="" />
        <img src="~assets/img/svg/qc.svg" alt="" /><img
          src="~assets/img/svg/pq.svg"
          alt=""
        />
        <img src="~assets/img/svg/avo.svg" alt="" />
        <img src="~assets/img/svg/qc.svg" alt="" /><img
          src="~assets/img/svg/pq.svg"
          alt=""
        />
        <img src="~assets/img/svg/avo.svg" alt="" />
        <img src="~assets/img/svg/qc.svg" alt="" /><img
          src="~assets/img/svg/pq.svg"
          alt=""
        />
        <img src="~assets/img/svg/avo.svg" alt="" />
        <img src="~assets/img/svg/qc.svg" alt="" /><img
          src="~assets/img/svg/pq.svg"
          alt=""
        />
        <img src="~assets/img/svg/avo.svg" alt="" />
        <img src="~assets/img/svg/qc.svg" alt="" /><img
          src="~assets/img/svg/pq.svg"
          alt=""
        />
        <img src="~assets/img/svg/avo.svg" alt="" />
        <img src="~assets/img/svg/qc.svg" alt="" /><img
          src="~assets/img/svg/pq.svg"
          alt=""
        />
        <img src="~assets/img/svg/avo.svg" alt="" />
        <img src="~assets/img/svg/qc.svg" alt="" /><img
          src="~assets/img/svg/pq.svg"
          alt=""
        />
        <img src="~assets/img/svg/avo.svg" alt="" />
        <img src="~assets/img/svg/qc.svg" alt="" /><img
          src="~assets/img/svg/pq.svg"
          alt=""
        />
        <img src="~assets/img/svg/avo.svg" alt="" />
        <img src="~assets/img/svg/qc.svg" alt="" />
      </div>
    </section>
    <div class="items_projets">
      <no-ssr>
        <vue-tiny-slider v-bind="tinySliderOptions" ref="tinySlider">
          <div class="item">
            <img src="~/assets/img/svg/mb.svg" alt="" />
            <p class="content_item">
              Sarah a le chic de donner de l’âme à tout ce qu’elle touche.
              Depuis qu’elle travaille avec nous en tant que « communnity
              manager », elle inonde nos réseaux de bonne humeur et de couleur
              plus qu’appréciées. L’enthousiasme qu’elle dégage est contagieux.
            </p>
            <p class="infos">O p’tit Quebec - Restauration</p>
          </div>
          <div class="item">
            <img src="~/assets/img/svg/mb.svg" alt="" />
            <p class="content_item">
              Sarah est professionnelle et réactive. Sa palette de compétences
              est très utile pour vos réseaux. De la photographie aux réseaux
              sociaux, Sarah améliore votre notoriété avec une image pro !
            </p>
            <p class="infos">Aurélien LABROT- Light Marketing</p>
          </div>
        </vue-tiny-slider>
      </no-ssr>
    </div>

  </section>
</template>

<script>
export default {
  data() {
    return {
      tinySliderOptions: {
        mouseDrag: true,
        loop: true,
        items: 1,
        nav: false,
        container: '.box_cards',
        autoplayButtonOutput: false,
        gutter: 80,
        autoplay: true,
        speed: 500,
        preventScrollOnTouch: 'auto',
        controls: true,
        prevButton: '#prev_p',
        nextButton: '#next_p',
        responsive: {
          1024: {
            items: 3,
            edgePadding: 40,
            loop: false,
            prevButton: '#prev_c',
            nextButton: '#next_c',
          },
        },
      },
    }
  },
  head() {
    return {
      link: [
        {
          rel: 'stylesheet',
          href: 'https://cdnjs.cloudflare.com/ajax/libs/tiny-slider/2.9.1/tiny-slider.css',
        },
      ],
    }
  },
}
</script>

<style scoped>


span {
  background-color: var(--green);
}

.client {
  position: relative;
    overflow: hidden;
  background: rgb(255, 255, 255);
  background: -moz-linear-gradient(
    180deg,
    rgba(255, 255, 255, 1) 0%,
    rgba(211, 233, 231, 1) 50%,
    rgba(255, 255, 255, 1) 100%
  );
  background: -webkit-linear-gradient(
    180deg,
    rgba(255, 255, 255, 1) 0%,
    rgba(211, 233, 231, 1) 50%,
    rgba(255, 255, 255, 1) 100%
  );
  background: linear-gradient(
    180deg,
    rgba(255, 255, 255, 1) 0%,
    rgba(211, 233, 231, 1) 50%,
    rgba(255, 255, 255, 1) 100%
  );
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr="#ffffff",endColorstr="#ffffff",GradientType=1);
  height: 800px;
  margin-bottom: 100px;
}

.box_client {
  text-align: center;
}

.box_client .content h3 {
  font-size: 28px;
  font-weight: 900;
  margin-top: 100px;
}

.box_client .content img {
  width: 130px;
  position: absolute;
  top: 20px;
  right: -10px;
}

.photof {
  position: absolute;
  top: 0;
  left: -30px;
  width: 80px;
}

.tocf {
  position: absolute;
  bottom: -10px;
  right: -30px;
  width: 140px;
}

.partenaires {
  margin: 80px 0 60px 0;
  overflow: hidden;
}

.box {
  display: flex;
  flex-flow: row nowrap;
  align-items: center;
  animation: slide 55s infinite linear;
}

@keyframes slide {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(-1000%);
  }
}

.box img {
  width: 170px;
  margin-right: 60px;
}

.items_projets {
  padding: 0 25px;
}

.item img {
  width: 110px;
}

.content_item {
  margin-top: 20px;
  font-size: 16px;
  line-height: 26px;
  color: var(--body);
  height: 190px;
  overflow: hidden;
}

.infos {
  font-weight: 900;
}

.btn button {
    text-align: center;
    display: flex;
    margin: 60px auto;
    width: 210px;
}

@media screen and (min-width: 1024px) {
  .box {
    display: flex;
    flex-flow: row nowrap;
    align-items: center;
    animation: slide 155s infinite linear;
  }
}

@media screen and (min-width: 1800px) {
  .box {
    display: flex;
    flex-flow: row nowrap;
    align-items: center;
    animation: slide 255s infinite linear;
  }

  .box img {
    width: 700px;
    margin-right: 50px;
  }
}
</style>
