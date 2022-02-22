<template>
  <section class="servicesIndex">
    <div class="story_services">
      <p>
        Dans la vie, j’ai 3 passions: manger, photographier ce que je mange, et
        le <span class="yellow">partager sur le web ! </span>C'est pourquoi je vous propose différents
        services.
      </p>
      <img src="~/assets/img/svg/trait.svg" alt="" />
    </div>

    <div class="items_services">
      <no-ssr>
        <vue-tiny-slider v-bind="tinySliderOptions" ref="tinySlider">
          <div class="item">
            <img src="~/assets/img/svg/photos.svg" alt="" />
            <p class="title_item">Photographie Culinaire</p>
            <p class="content_item">
              Je mets en valeur vos produits grâce à des photos stylisées et
              personnalisées.
            </p>
            <p class="infos">En savoir plus</p>
          </div>
          <div class="item">
            <img src="~/assets/img/svg/coms.svg" alt="" />
            <p class="title_item">Communication</p>
            <p class="content_item">
              Je vous accompagne dans la réalisation de votre stratégie de
              communication.
            </p>
            <p class="infos">En savoir plus</p>
          </div>
          <div class="item">
            <img src="~/assets/img/svg/socials.svg" alt="" />
            <p class="title_item">Social Média</p>
            <p class="content_item">
              Je vous accompagne dans la réalisation de votre stratégie social
              media.
            </p>
            <p class="infos">En savoir plus</p>
          </div>
          <div class="item">
            <img src="~/assets/img/svg/creas.svg" alt="" />
            <p class="title_item">Création de contenu</p>
            <p class="content_item">
              Je parle de votre marque/vos produits sur le blog et sur les
              réseaux sociaux.
            </p>
            <p class="infos">En savoir plus</p>
          </div>
          <div class="item">
            <img src="~/assets/img/svg/coms.svg" alt="" />
            <p class="title_item">Création recettes</p>
            <p class="content_item">
              Je crée et partage des recettes gourmandes à partir de vos
              produits.
            </p>
            <p class="infos">En savoir plus</p>
          </div>
        </vue-tiny-slider>
      </no-ssr>
    </div>
    <div class="slide_prev_next">
      <div class="prev" id="prev_p">
        <img src="~/assets/img/svg/prev.svg" alt="" />
      </div>
      <div class="next" id="next_p">
        <img src="~/assets/img/svg/next.svg" alt="" />
      </div>
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
        gutter: 0,
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
            prevButton: '#prev_p',
            nextButton: '#next_P',
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
.servicesIndex {
  padding: 0 10px;
  margin-bottom: 50px;
}

.story_services {
  text-align: center;
}

.story_services p {
  padding: 0 10px;
  color: var(--body);
  font-style: italic;
  font-size: 16px;
  line-height: 24px;
  margin-bottom: 10px;
}

.yellow {
  background-color: var(--yellow)!important;
  font-weight: 700;
  color: var(--black);
}

.items_services {
  text-align: center;
  margin-top: 50px;
}

.item .title_item {
  margin: 15px 0;
  font-size: 18px;
  font-weight: 900;
}

.content_item {
  width: 270px;
  line-height: 24px;
  margin: auto;
  color: var(--body);
}

.infos {
  margin: 20px 0;
  color: var(--black);
  font-weight: bold;
}

.slide_prev_next {
  display: flex;
  justify-content: center;
  margin-top: 30px;
  margin-bottom: 50px;
}

.prev {
  margin-right: 10px;
}

.btn {
  margin: 20px 0;
  text-align: center;
}
</style>
